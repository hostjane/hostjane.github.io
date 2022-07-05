---
layout: default
title: 1-Click LEMP
parent: Cloud Computes
description: How to setup an Ubuntu server
nav_order: 4
permalink: /cloud-compute/lemp-setup/
---

# 1-Click LEMP

<span class="yellow">This tutorial helps you run the latest LEMP version on HostJane Cloud computes, which is comprised of:</span>

- [x] L for Linux
- [x] E is for Nginx (engine-x),
- [x] M is for MariaDB or MySQL
- [x] P for PHP

<span class="orange">LEMP can run on Ubuntu and CentOS.</span>

1. TOC
{:toc}

## 1. Get server IP and root password

After successful payment is approved, your server will be set up within 2 minutes.

### A. Login to the Hosting Portal

Bookmark login: [https://console.hostjane.com/client/login](https://console.hostjane.com/client/login)

In your Dashboard under Services, find your LEMP server.

| Package | Label | Term  | Date Created | Date Renews | Options |
|:-------|:----------|:------|:----------|:------|:------|
| LEMP | host.domain.com | 1 month @ $0.00 | Jan 1 | Feb 1 |*Manage* |

We offer 24×7×365 support

If you cannot see your LEMP service, open a support case.

### B. Click the Manage option

This is the button in the last column under Services.

Here is the next screen that will display: 

| Package | Status|
|:-------|:----------|
| LEMP | Active|
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

## 3. Access your server in the browser

In this example, the server link is: https://123.456.789.1

In this example case the IP is: 123.456.789.1

```
Your Server Link:
https://[Your_Server’s_IP]/
```

For security, HostJane does not send this to you by email.

When you first access your server IP in a browser, you should see HostJane’s default HTTP server test page. You may also see a Vultr branded page depending on your datacenter.

This denotes correct NGINX configuration.

![](/assets/hosting/lemp-server-config-default.png)

Successfully viewing this page in the browser indicates that the NGINX server can serve web pages and is working properly.

Replace this test page with your own contents by navigating to /usr/share/nginx/html in your server’s file directory.

## 4. Ignore the browser warning

### A. Copy and paste your unique server link 

Open a fresh browser window and paste the link

Hit Enter.

### B. Find the HTTPS warning

The warning can be safely ignored.

It will look slightly different depending on which browse you're using. In Chrome it may appear like this:

![](/assets/hosting/ssl-warning-janevps-chrome.jpeg)

In Mozilla Firefox, it may look like this:

![](/assets/hosting/ssl-warning-janevps-2.jpeg)

Click the Advanced or Add Exception link to accept the warning and proceed to the unsafe page.

A security dialog box will open.

![](/assets/hosting/login-to-HTTPS-server.png)

Enter the username and password credentials into the box, as found in Statistics.

Click Sign in or Enter.

### Why is there a warning?

HostJane cannot configure an SSL certificate (HTTPS://) for an IP address on its own. We need to wait until your domain is pointing to the server, and then assign your FREE SSL certificate to your domain.

<span class="green"> Until your domain's A-record is setup, whenever you access your server by HTTPS://, a warning appears in your browser.</span>

Your server comes with a self-signed SSL certificate.

If you access the server link using HTTP://, you will not see the warning. 

### C. How to remove the SSL warning

Once your domain's A-record is successfully pointing to your server, HostJane can install your FREE SSL certificate to remove the warning.

Request your FREE SSL certificate

Open a support ticket after your domain is pointed correctly to your server.

You can check when propagation is successful by doing a DNS lookup of your domain's A-record.

Please note that we can only install an SSL certificate on a top-level domain (TLD)

For example: https://www.yourdomain.TLD, where the TLD could be .com, .net, .org, .ca, or any TLD available.

HostJane and our servers work with all domain registrars worldwide.

## 5. Locating the web document root

After logging in on the root, you can upload files (e.g. html and php) to:

```
/usr/share/nginx/html/
```

Files uploaded to this directory will take the URL structure:

```
http://[Your_Server’s_IP]/[Uploaded_File]
```

## 6. Access the MySQL database on LEMP servers

You can connect to the MySQL database by running:

```
mysql -u root
```

The MySQL root password is saved at:

```
/root/.my.cnf
```

You now have the basic information to start using your new server running LEMP and begin installing any software.