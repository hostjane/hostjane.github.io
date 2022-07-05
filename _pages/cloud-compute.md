---
layout: default
title: Cloud Computes
description: Cloud Hosting docs and help tutorials
nav_order: 7
has_children: true
permalink: /cloud-compute/
---

# HostJane Cloud Computes

<span class="green">Scalable, linux-based virtual machines deployed in 2 minutes. Each compute includes full management, DDoS protection, fast Intel® cores and SSD storage.</span>

1. TOC
{:toc}

## Cloud Features

| Feature |	Description |
|:-------------|:------------------|
| Managed | Each compute instance runs as a virtualized layer above world-class hardware—root access and a unique dedicated IPv4 and IPv6 (optional) address. 24×7 monitoring, server and app support included free, that larger unmanaged and self-managed cloud providers bill as "add-ons". |
| 24 Hr Backups | On HostJane Cloud’s 10Gbit network, for an additional fee we can automatically backup your cloud server every 24-48 hours. Two backups will always available as “restore points”. Your data is protected in Tier III world-class datacenters. Open a support case to request a list of backups available. *We charge an up-front $15 data restore fee for administration work to restore a HostJane Cloud to an earlier time.* |
| 10 GBIT NETWORK | HostJane Cloud’s resilient network offers good and transparent uptime, fantastic global connectivity, and Tier III datacenters that operate: 24/7 IT experts proficient in public and private cloud security; Robust, state-of-the art facilities that guard against both natural disasters and physical intrusions; Back-up generators |
| Snapshots	| It’s easy to create a copy or snapshot of your HostJane Cloud server at a specific moment in time, for future backup or prior to major changes. Developed with top datacenters, the infrastructure is consistently improving. |
| Private Spaces | Not ready to go live? We can move your server behind a cloud firewall, which is a secure location in the datacenter. Only you, our support team, and your handpicked IP whitelist will be granted access to see your cloud while it’s in private space. |
| DDoS Protection | HostJane protects against multiple types of Denial-of-Service actions designed to overwhelm your server. We guard against up to 10 GB per second of malicious traffic against your HostJane Cloud and associated IP addresses. The HostJane Cloud network continuously analyzes all traffic and will filter and attenuate malicious Denial-of-Service attacks, diverting malicious traffic to a mitigation zone as soon as bad actors are identified on the network. **Customers should be aware that no system however protected is DDoS proof. HostJane Cloud’s network will protect you against the most common volume-based and protocol floods.** |
| Scale Instantly | HostJane Clouds are deployed in 90-120 seconds with full CLI root-access, and scale instantly with no downtime. If your website takes an unexpected surge of traffic, HostJane Cloud will keep you up.** |

**Additionally, HostJane Clouds include a suite of proactive fully-managed services to support fast scaling:

1. Seamless, instant cloud scaling on request;
2. 24-hr auto backups available with free backup storage;
3. 24×7 monitoring;
4. Qualified 24×7 response team;
5. On-going maintenance;
6. OS updates and patches;
7. Cyber security and server hardening;
8. Regular server audits ensuring the platform won’t let you down.

### Bandwidth overages

You will receive an email informing you to upgrade your server and offering options.

If not practical, the server will be stopped.

## Fully-Managed

HostJane Cloud assists cost-savvy business teams with a live production server including 24×7 incident response, automatic OS patches & upgrades. Get on your project and let us worry about keeping your server in peak condition.

| Feature |	MANAGED | UN-MANAGED | SELF-MANAGED |
|:-------------|:------------|:------|:------|
| Fully-managed VMs with application support | Y | N | N |
| 24×7 Incident Response Team |	Y |		N |		N |
| Production ready |		Y |		N |		N|
| Full-Stack Support; (*incl. LEMP and LAMP servers***)  |		Y |		N	 |	N|
| Proactive Service Monitoring |		Y	 |	N |		N|
| Nightly Backups |		Y / Fees apply |		N |		N|
| Free Firewalls |		Y |		NO |		Varies|
| Included DDoS Protection |	Y	 |	Varies |		NO|
| Free snapshots |	Y |		NO	 |	Varies|
| Included Outgoing Bandwidth 	 |	Y	 |	NO |		NO|
| Allowed IPv4 Addresses	 |	1 IPv4 Included; 1 IPv6 Included; +IPv4 (+$4/mo) |		Up to 16 IPv4	 |	Varies|
| Predictable Billing |		Y	 |	N |		N|
| Control panel & Stats	 |	Y	 |	Y	 |	Y|
| Root access	 |	Y	 |	Y	 |	Y|
| RESTful API	 |	NO |		Y |		Y|
| DNS Manager	 |	NO |		Y |		Y|

<span class="blue">**If you run a HostJane Cloud LAMP or LEMP stack (or install the stack yourself) we’ll manage it for you. We’ll also take care of important OS patches, daily server maintenance, and respond to any problem with 24×7 support.</span>

## Root access

Yes. Login to the Hosting Portal and use your server’s IP address provided in Statistics 

Connect to your HostJane Cloud server either with PuTTY on Windows or an OpenSSH client in linux and MacOS devices.

### A) Open your client terminal

Enter the command:

```
ssh root@[Your_Server's_IP]
```

You need to replace `[Your_Server's_IP]` with your HostJane Cloud’s IP address from Statistics in the Hosting Portal after the @

Hit enter and yes to any prompts.

### B) Enter root password

Unless you are connecting with SSH keys, you need to manually enter the root password (found in your server’s Statistics dashboard in the Hosting Portal) to complete the login.

## Help setting up

Refer to HostJane Cloud Setup Guides or hire a developer on HostJane Marketplace

These cover basic techniques for running basic linux distributions like Ubuntu and CentOS, and help using PuTTY and other command line programs.

Unfortunately our staff are not able to provide in-depth consultations.

We also recommend looking into some linux courses offered by IT tutors on HostJane Marketplace if you need extra assistance.

## Domain pointing

You will need to add an A-record to your domain at the registrar.

## Large size computes

Yes, we can offer full-managed linux clouds over 160GB including upgrading your current cloud.

We will need to verify your account by signing a credit card authorization form with copies of front and back of your card.

Please contact us for pricing or open a ticket if you’re an existing customer.

## Reboots

1. Login to your HostJane Cloud server in the Hosting Portal

| Package | Label | Term  | Date Created | Date Renews | Options |
|:-------|:----------|:------|:----------|:------|:------|
| Service | host.domain.com | 1 month @ $0.00 | Jan 1 | Feb 1 |*Manage* |

Click Manage Server

| Package | Status|
|:-------|:----------|
| Service | Active|
| **Label** | **Renew Date**|
| host.domain.com | Feb 1 |
| **Creation Date** | **Next Invoice**|
| Jan 1 | Feb 1 |
| **Billing Cycle** | **Recurring Amount**|
| 1 Month | $0.00 |

In the sidebar, navigate to: Manage > Server > Actions

Click the green restart button.

## Static IP

Yes, it can’t be changed even if you buy a second IPv4 or a floating IPv4.

To set a new IPv4, you'd need to spin up a new cloud server.

## Windows-based servers

Unfortunately we do not offer any Windows products at this time.

## Additional IPs

At this time, you can purchase 1 additional IPv4 address per HostJane Cloud. Open a support ticket to buy an IPv4.

## Automatic Backups

HostJane can provide a nightly backup of your entire server files and databases for an additional fee. There is no extra cost for backup storage.

We will then always have at least 2 past backups of each HostJane Cloud in our system.

We begin overwriting past backups, after 72 hours of storage. To request a restoration from a past backup, please contact us. There is a $15 data restore admin fee.

*Note the restoration process can take up to 60 minutes and during that time your server may be unavailable.*

## Billing policy

All HostJane Cloud VMs must be paid for at the beginning of the monthly billing cycle.

## Refund policy

Due to the nature of cloud server provisioning, refunds are typically not available unless there is a material problem with your server that occurs our end.

## SSH keys

Yes, HostJane Cloud supports SSH keys

Once you have generated your keys in PuTTYgen, use your terminal client to add the public key (which is the long string beginning ssh rsa) to the root user on your HostJane Cloud server.

Create a PuTTY Profile to login without using your password

<span class="red">WARNING: Make sure you do not lose your keys as we cannot help you recover them if lost. If you’ve disabled username/password login you won’t be able to login to your server.</span>

## Connect via SFTP

Yes, read our FTP guide.

## Lost SSH passwords

For security reasons, we have to reset the root password for you. However, this attracts a small admin fee. Contact support to proceed.

## Cancellation

Hosting customers can destroy their servers from the secure Hosting Portal.

This will automatically cancel the service, but does NOT provide a prorated refund if you cancel before the end of the monthly cycle.

1. Login to your My HostJane account and navigate to the Dashboard. Find the server you wish to destroy in the server list.
2. Select *Manage* under Options.
L3. ook for Cancel Server at the bottom of the Information tab.
4. Select *Cancel Options*
5. You can choose to cancel immediately or at the end of the current monthly term. You will need to confirm your Hosting Portal account password to proceed with termination.

<span class="red">Cancellation is immediate and not reversible. All data is destroyed.</span>

# Connecting to your server with PuTTY (Windows)

[PuTTY](https://www.putty.org/) is an SSH and Telnet client that lets you connect to your server on the command line (CLI) in Windows machines.

## How to get PuTTY

<span class="green">You can [download PuTTY](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html) at its creator’s website with x32 and x64 Windows versions available.</span>

Download the .msi file and follow instructions to install PuTTY on your windows machine.

## 1. Open PuTTY

Type your server’s IP address in the Host Name field under:

### A. Basic options for your PuTTY session:

![](/assets/hosting/Putty-interface.png)

Ensure the PuTTY port is 22

### How to find your server IP?

Login to the Hosting Portal > locate your server plan and click the Manage button.

In the example below we are using a CentOS server.

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

## 2. Add SSH keys to PuTTY (Optional)

If you have already created your SSH private keys with .ppk extension in [PuTTYgen](http://www.chiark.greenend.org.uk/~sgtatham/putty/download.html), upload these into PuTTY.

In the left-hand tree, go to SSH > Auth:

![](/assets/hosting/ssh-keys-putty.png)

In the left-hand tree, go to Connection > Data.

The first-time you login enter root as the auto-login username to be sent to the server.

On subsequent logins, after you’ve set up your server you can add new users to saved logins.

For example sudo users you’ve given root privileges to.

![](/assets/hosting/connection-data-putty.png)

Finally, in the left-hand tree, return to Sessions

Enter a name of your session in the Saved Sessions box, for example, JaneDoe (or another name you wish to use) to remember your login credentials.

Click Save to add this session ID to the list.

![](/assets/hosting/saved-sessions.png)

Your SSH-enabled username is now saved by the PuTTY client for repeated SSH login use.

Click Load with JaneDoe to begin a new session with your saved SSH credentials.

## 3. Connect to server for the first time

You must manually trust the server.

When you connect for the first time with your PuTTY client in Windows to a new server, you can opt to save the **server’s identity** to the cache of your PuTTY client.

![](/assets/hosting/putty-fingerprint-cache.png)

Click Yes to trust the server and save the identity.

You’ll only need to do this once.

If you used SSH keys, you will be connected directly to your server without being prompted further for a password.

In all other case, you'll need to enter your login and password to proceed.

![](/assets/hosting/login-server-putty.png)

# Connect with OpenSSH on Linux or macOS

### Linux users

Whether you’re on a MacOS or Linux operating system, you will need to open an SSH terminal.

In linux systems like  Ubuntu, this can usually be done by pressing:

Ctrl + alt + t or searching “terminal”.

#### Basic definitions

- **Console** – This means your entire system including display monitor, input device (like keyboard and mouse) and the command line terminal that will talk to the server.

- **Command line shell** (CLI, command line interface or terminal) – This is the text interface where you type commands to control what actions your remote server at HostJane performs. It’s the software program we use to connect to the remote server at HostJane. It’s also called a terminal emulator because it copies the functions of the old-school classic computer terminal inside your modern Mac or Linux desktop.

- **Prompt** – At the beginning of the command line, you will see information about your user status, which folder in the operating system’s directory you are currently located, ending with a `$`

For example: `[ janedoe@123.456.789.1: ~janedoe $ ]`

This entire line makes up the prompt

- **Bash** – This stands for Bourne Again shell, it’s the standard shell or terminal that ships with every MacOS device and is found on most linux systems.

## Mac users

In Apple MacOS machines, open Applications in Finder or LaunchPad, then go to the folder Utilities where the terminal icon can be found.

![](/assets/hosting/applications-folder.png)

**Go to Utilities and select Terminal**

![](/assets/hosting/terminal-mac.png)

If you still can’t find it, try doing a search on your MacOS for “terminal”

![](/assets/hosting/search-spotlight-terminal.png)

## 1. Login into the server

Once the terminal is open, use the SSH command to login to your server:

```
ssh user@[Your_Server's_IP]
```

Replace `Your_Server’s_IP` with the server IP address given in Statistics.

Now enter:

```
ssh root@[Your_Server's_IP]
```

See the second line in this example:

![](/assets/hosting/janedoe-ssh-login.png)

If you already have set up your SSH keys and they are present on your Mac device, use the -i command and type the full pathway to where the key is present:

```
ssh -i /path/to/private/key username@203.0.113.0
```

The terminal should return:

```
The authenticity of host '203.0.113.0 (203.0.113.0)' can't be established.

ECDSA key fingerprint is SHA256:[Unique_Fingerprint].
```

You’ll be asked to confirm you want to proceed, type `yes`

```
Are you sure you want to continue connecting (yes/no)? yes
```

The host fingerprint will be saved to your local device:

```
Warning: Permanently added '123.456.789.1' (ECDSA) to the list of known hosts.
```

If you’re using SSH keys, you will be logged in if with no further prompts.

Otherwise, you’ll be prompted to enter your root password:

```
root@123.456.789.1's password:
```

Either manually type enter your password and press:

- On Ubuntu: Ctrl + shift + v
- On MacOS: Shift + command + v

You should now be logged into your server through the SSH terminal.

## 2. Remove the warning message

Quite commonly the following warning can show if a host SSH key is not removed properly from your local device.

This occur if you connect to a new server with the old key still on your local device operating system

```
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@ WARNING: REMOTE HOST IDENTIFICATION HAS CHANGED! @
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
IT IS POSSIBLE THAT SOMEONE IS DOING SOMETHING NASTY!
Someone could be eavesdropping on you right now (man-in-the-middle attack)!
It is also possible that the RSA host key has just been changed.
```

To resolve this, flush the old key by typing:

```
ssh-keygen -R [Your_Server's_IP]
```

Then log back into the server with the root user and new SSH key details.

# Connect via FTP

#### HostJane recommends FileZilla

1. FileZilla is a simple-to-use, free File Transfer Protocol (FTP) solution to modify and upload to specific file directories on your server.
2. You cannot remotely extract compressed files with Filezilla (i.e. .zip files), which needs to be done on the command line.

## 1. Download FileZilla

Download the latest [FileZilla version](https://filezilla-project.org/download.php?type=client) here, Filezilla will detect automatically what operating system you are using.

![](/assets/hosting/filezilla-mac.png)

## 2. Connect to server by root 

Open FileZilla after installation, and you will see 4/5 panels.

On Windows systems, it looks like this:

![](/assets/hosting/file-zilla.png)

Enter the following credentials to connect as root user to your server:

```
**Host**: sftp:/[/Your_Server_IP] (or your hostname i.e. host.yourdomain.com)
**Username**: root
**Password**: [root password]
**Port**: 22
```

This is given in Statistics in [Console](https://console.hostjane.com)

Click Quickconnect to login, and the credentials will be stored for future use.

Click yes to any prompts

For example: *“You have no guarantee that the server is the computer you think it is”*

![](/assets/hosting/host-prompt-sftp.png)

You should then see a message showing:

```
Status: Retrieving directory listing…
Status: Listing directory /root
Status: Directory listing of "/root" successful
```

You can now manipulate files in the right-hand window showing /root directory as shown below:

![](/assets/hosting/logged-in-filezilla.png)