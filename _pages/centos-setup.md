---
layout: default
title: 1-Click CentOS
parent: Cloud Computes
description: How to setup a LAMP server
nav_order: 6
permalink: /vps-hosting/centos-setup/
---

# 1-Click CentOS

<span class="green">Tutorial for running latest CentOS version on HostJane cloud servers.</span>

1. TOC
{:toc}

## Production-ready requirements

We recommend several steps before you install any software layer onto the new environment.

This is an important security step if you are intending on using your server for production projects.

## 1. Get server IP and root password

After successful payment is approved, your server will be set up within 2 minutes.

### A. Login to the Hosting Portal

Bookmark login: [https://console.hostjane.com/client/login](https://console.hostjane.com/client/login)

In your Dashboard under Services, find your CentOS server.

| Package | Label | Term  | Date Created | Date Renews | Options |
|:-------|:----------|:------|:----------|:------|:------|
| CentOS | host.domain.com | 1 month @ $0.00 | Jan 1 | Feb 1 |*Manage* |

We offer 24×7×365 support

If you cannot see your CentOS service, open a support case.

### B. Click the Manage option

This is the button in the last column under Services.

Here is the next screen that will display: 

| Package | Status|
|:-------|:----------|
| CentOS | Active|
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

**Replace janedoe with the unique name of your new user.****

Set a new password for janedoe

```
passwd janedoe
```

At the prompt, reenter the new password and confirm by pressing Enter

## 4. Add super-user privileges

Add janedoe to the wheel group to assign super-user privileges to the user.

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

With the SSH key now installed, log back into your cloud server using your new janedoe user.

```
ssh -1 janedoe Your_Server's_IP
```

Login should be successful.

Close all other open terminals.

## 6. Disable root user login

Edit the SSH daemon configuration to prevent anyone logging into your server using the root or password authentication.

Use nano, the command-line text editor, to open the SSH daemon file (after logging in with your SSH new super user) by typing:

```
sudo nano /etc/ssh/sshd_config
```

Find `PermitRootLogin`, it will look like this:

```
PermitRootLogin yes
```

Set it to no using your cursor

```
PermitRootLogin no
```

Check that PasswordAuthentication in the same SSH daemon file is also set to `no`

```
PasswordAuthentication no
```

Press `ctrl + O` then Enter to write the changes to SSH daemon

Now close the file with `ctrl + x`

## 7. Reload SSH

To save the changes, restart the SSH service:

```
sudo systemctl reload sshd
```

## 8. Set the server time zone

Edit the `/usr/share/zoneinfo` directory

Pull up a list of your server's timezones by running:

```
ls -R /usr/share/zoneinfo
```

You’ll see an output, such as:

![](/assets/hosting/usr-timezones.png)

Use sudo command to change your timezone:

```
sudo ln -sf /usr/share/zoneinfo/Time/Zone /etc/localtime
```

Replace `/Time/Zone` with your actual location’s timezone, e.g. /US/Arizona

```
sudo ln -sf /usr/share/zoneinfo/US/Arizona /etc/localtime
```

Now run the `date` command to test that your janeCloud’s timezone is updated.

```
date
```

If successful, the output will give you Arizona (GMT -7) time:

```
Day Month Day 00:00:00 MST Year
```

Your CentOS server is now reasdy to use!