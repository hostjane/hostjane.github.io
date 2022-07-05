---
layout: default
title: 1-Click Debian
parent: Cloud Computes
description: How to setup an Ubuntu server
nav_order: 2
permalink: /cloud-compute/debian/
---

# 1-Click Debian

<span class="yellow">The following tutorial is designed to help you run the latest Debian version on HostJane computes.</span>

1. TOC
{:toc}

## Production-ready requirements

We recommend several steps before you install any software layer onto the new environment. This is an important security step if you are intending on using your server for production projects.

## About Debian

Debian is a powerful open-source linux distribution that is easy to install and secure.

Debian is the base for Ubuntu.

## 1. Get server IP and root password

After successful payment is approved, your server will be set up within 2 minutes.

### A. Login to the Hosting Portal

Bookmark login: [https://console.hostjane.com/client/login](https://console.hostjane.com/client/login)

In your Dashboard under Services, find your Debian server.

| Package | Label | Term  | Date Created | Date Renews | Options |
|:-------|:----------|:------|:----------|:------|:------|
| Debian | host.domain.com | 1 month @ $0.00 | Jan 1 | Feb 1 |*Manage* |

We offer 24×7×365 support

If you cannot see your Debian service, open a support case.

### B. Click the Manage option

This is the button in the last column under Services.

Here is the next screen that will display: 

| Package | Status|
|:-------|:----------|
| Debian | Active|
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

**Replace janedoe with the unique name of your new user.**

You will be automatically asked to set a new password for janedoe, and to reenter the password to confirm.

Press Enter to proceed with default information, otherwise enter values for your:

1. Full name
2. Room number
3. Work phone
4. Home phone
5. Other

## 4. Install sudo on Debian

Add janedoe to the sudo group to assign super-user privileges to the user.

We first need to install sudo, using the command apt-get

Type:

```
apt-get update
```

When the apt package has finished updating, install sudo with:

```
apt-get install sudo
```

You should still be logged in as the root user.

Now we can use `sudo` commands to give the new user, janedoe, root privileges:

```
usermod -a -G sudo janedoe
```

You can now run janedoe with the same level of access as the root user.

## 5. Set up public SSH keys

We recommend you set up an SSH key pair to secure your server.

SSH key setup is easy and free, but if you're not comfortable doing this we recommend hiring a system administrator on HostJane Marketplace.

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

## 6. Switch to new user to enter home directory

Substitute janedoe for the user you created in step 3.

```
su - janedoe
```

Create a new directory .ssh and restrict permissions:

```
mkdir ~/.ssh
```

Ensure there are no spaces between / and .ssh

```
chmod 700 ~/.ssh
```

Use nano, the command-line text editor, to edit the authorized_keys file in .ssh directory by typing:

```
chmod 600 ~/.ssh/authorized_keys
```

Type exit to switch back to the root user.

## 7. Verify the configuration

Check that janedoe can successfully log into the server using SSH.

Enter:

```
SSH janedoe@[Your_Server's_IP]
```

If successful, you will login to your server using your private key and will not be prompted for a password.

## 8. Disable root login

Only disable root logins if you have set up SSH keys on the server, otherwise you’ll be locked out.

Edit the SSH daemon file to prevent unauthorized users logging into your server using password authentication.

Login by SSH to your server with your new super-user, for example, janedoe

Use nano, the command-line text editor, to open the SSH daemon file:

```
sudo nano /etc/ssh/sshd_config
```

Find PermitRootLogin, it will look like this:

```
PermitRootLogin yes
```

Set it to no using your cursor

```
PermitRootLogin no
```

Press `ctrl + O` then Enter to write the changes to SSH daemon

Now close the file with `ctrl + x`

## 9. Reload SSH

To save the changes, restart the SSH service:

```
sudo systemctl restart sshd
```

You are now ready to start using your new Debian compute!