---
layout: default
title: 1-Click Fedora
parent: Cloud Computes
description: How to setup an Ubuntu server
nav_order: 3
permalink: /cloud-compute/fedora/
---

# 1-Click Fedora

<span class="green">Tutorial for running latest Fedora version on HostJane cloud servers.</span>

1. TOC
{:toc}

## Production-ready requirements

We recommend several steps before you install any software layer onto the new environment. This is an important security step if you are intending on using your server for production projects.

## About Fedora

- [x] Developed on a six-monthly release cycle, Fedora is an open-source, widely-used linux operating system that is purposed as a downstream breeding ground and test center of code ideas to fuel Red Hat Linux Enterprise features.
- [x] Choosing Fedora over Ubuntu generally depends on what you need to do with your linux system.
- [x] As Fedora drops support for older versions every 6 months (with twice yearly releases), if your project requires running a long-term linux server, you may be better off with Ubuntu or CentOS. 
- [x] Some people who prefer not to learn the Debian Package Management system find Fedora more straightforward to manage.

## 1. Get server IP and root password

After successful payment is approved, your server will be set up within 2 minutes.

### A. Login to the Hosting Portal

Bookmark login: [https://console.hostjane.com/client/login](https://console.hostjane.com/client/login)

In your Dashboard under Services, find your Fedora server.

| Package | Label | Term  | Date Created | Date Renews | Options |
|:-------|:----------|:------|:----------|:------|:------|
| Fedora | host.domain.com | 1 month @ $0.00 | Jan 1 | Feb 1 |*Manage* |

We offer 24×7×365 support

If you cannot see your Fedora service, open a support case.

### B. Click the Manage option

This is the button in the last column under Services.

Here is the next screen that will display: 

| Package | Status|
|:-------|:----------|
| Fedora | Active|
| **Label** | **Renew Date**|
| host.domain.com | Feb 1 |
| **Creation Date** | **Next Invoice**|
| Jan 1 | Feb 1 |
| **Billing Cycle** | **Recurring Amount**|
| 1 Month | $0.00 |

### C. Click *Statistics* in the side menu

| Field | Value |
|:-------|:----------|
| Main IP | 123.456.789.1 |
| Default password | demo123 |

The Main IP is your virtual machine's IP address.

The Default Password is the root password.

For security, HostJane does not send this to you by email.

You must login to your hosting account to review these credentials.

## 2. Login with SSH

Login to your server with PuTTY on Windows or an OpenSSH client in linux and MacOS devices:

```
ssh -l root [Your_Server's_IP]
```

Replace `Your_Server’s_IP` with the server IP address given in Statistics.

## 3. Create a new user

For security reasons it’s best not to use the root user for everyday administrative tasks.

The solution is to create a new user.

Enter the following:

```
adduser janedoe
```

Replace `janedoe` with the unique name of your new user.

Set a new password for janedoe

```
passwd janedoe
```

You will be automatically asked to set a new password for janedoe, and to reenter the password to confirm.

You should then see confirmation:

```
passwd: all authentication tokens updated successfully
```

## 4. Add super-user privileges

Add `janedoe` to the wheel group to assign super-user privileges to the user.

```
gpasswd -a janedoe wheel
```

Your new user can now have root privileges using sudo commands.

## 5. Set up public SSH keys

We recommend you set up an SSH key pair to secure your server.

<span class="purple">SSH key setup is easy and free, but if you're not comfortable doing this we recommend hiring a system administrator on HostJane Marketplace.</span>

After you’ve set up your SSH keys, open another terminal on your local machine.

Add your SSH key to janedoe‘s home directory via the new terminal.

```
ssh-copy-id janedoe@Your_Server's_IP
```

## 6. Verify the configuration

Check that `janedoe` can successfully log into the server using SSH.

Enter:

```
SSH janedoe@[Your_Server's_IP]
```

If successful, you will login to your server using your private key and will not be prompted for a password.

## 7. Disable root user login

Edit the SSH daemon configuration to prevent anyone logging into your server using the root or password authentication.

Use nano, the command-line text editor, to open the SSH daemon file (after logging in with your SSH new super user) by typing:

```
sudo nano /etc/ssh/sshd_config
```

Find `PermitRootLogin`, it will look like this:

```
PermitRootLogin yes
```

Set it to `no` using your cursor

```
PermitRootLogin no
```

Check that PasswordAuthentication in the same SSH daemon file is also set to `no`

```
PasswordAuthentication no
```

Press `ctrl + O` then Enter to write the changes to SSH daemon

Now close the file with `ctrl + x`

## 8. Reload SSH

To save the changes, restart the SSH service:

```
sudo systemctl reload sshd
```

## 9. Enable the firewall

Protect your new Fedora server by enabling the iptables firewall and ensure that the firewall application continues to function after you reboot the server.

Ensure you are logged into your server as your super-user, e.g. janedoe.

We can enable the iptables package by first installing `iptables-services`:

```
sudo yum install -y iptables-services
```

![](/assets/hosting/fedora-iptables-services.png)

Next, ensure that iptables starts on boot:

```
sudo systemctl enable iptables
```

Next, start iptables:

```
sudo systemctl start iptables
```

View the default iptables rules on your Fedora server by typing:

```
sudo iptables -L
```

![](/assets/hosting/iptables-default-rules-fedora.png)

To save the rules, which will permit SSH traffic, type:

```
sudo /usr/libexec/iptables/iptables.init save
```

Now after you reboot, these ssh firewall rules will persist.

You should see confirmation:

![](/assets/hosting/iptables-firewall-save-fedora.png)

You are now ready to start using your new Fedora compute!