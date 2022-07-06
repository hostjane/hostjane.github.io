---
layout: default
title: 1-Click CentOS Web Panel
parent: VPS Hosting
description: How to setup a CentOS Web Panel VPS on HostJane
nav_order: 5
permalink: /vps-hosting/centos-web-panel/
---

# 1-Click CentOS Web Panel (CWP)

Manage you or your client's websites with CWP, a free, open-source web hosting control panel. CWP is an alternative to cPanel, enabling web host management without needing to touch a command line.

1. TOC
{:toc}

The user panel is feature-rich enabling you to manage your website's files, cron jobs, backups and more. 

A server with at least 2GB RAM is required

## 1. Point your domain to the server

The first step is create an A-record at your domain registrar.
This enables you to access your server in any browser at your web domain.

<span class="blue">Please note that it can take up to 72 hours for a domain to propagate throughout the internet to a server, although it usually happens much sooner.</span>

We can’t set up your FREE SSL certificate until this step is completed.

## 2. Obtain your server’s details

### A. Login to the Hosting Portal

Bookmark login: https://console.hostjane.com/client/login

In your Dashboard under Services, find your CentOS Web Panel server.

| Package | Label | Term  | Date Created | Date Renews | Options |
|:-------|:----------|:------|:----------|:------|:------|
| CentOS Web Panel | Domain.com | 1 month @ $0.00 | Jan 1 | Feb 1 |*Manage* |

We offer 24×7×365 support

If you cannot see your WordPress service, open a support case.

### B. Click the Manage option

This is the button in the last column under Services.

Here is the next screen that will display: 

| Package | Status|
|:-------|:----------|
| CentOS Web Panel | Active|
| **Label** | **Renew Date**|
| Domain.com | Feb 1 |
| **Creation Date** | **Next Invoice**|
| Jan 1 | Feb 1 |
| **Billing Cycle** | **Recurring Amount**|
| 1 Month | $0.00 |

### C. Click Statistics in the menu

Your private and confidential server root password and IP address is in *Statistics*.

Security Alert

Never disclose, email, or publish your password to anyone, including HostJane staff in support tickets. Our technicians have safe access inside secure datacenters if they need this.

Below is a example screenshot of the Application Information.

| CentOS Web Panel Server Details|
|:-------|
| Access CentOS Web Panel at the following URL |
| `https://123.456.789.1:2031` |
| `User: root` |
| `Pass: (server root password)` |

In this example, the server link is: https://123.456.789.1:2031

The first set of numbers before the :2031 is your server IP address.

In this example case the IP is: 123.456.789.1

Your Server Link
https://[Your_Server’s_IP]:2031

For security, HostJane does not send this to you by email.

You must login to your hosting account to review these credentials.

## 3. Ignore the browser warning

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

## 4. Access the CWP Installer

Copy and paste the installer link into a fresh browser window.

The installer address will look something like this, but will have your server’s IP address:

https://[Your_Server’s_IP]:2031

Replace Your Server’s IP with your CentOS Web Panel server’s IP as found in Statistics

For example:

https://123.456.789.1:2031

For your security we don’t send this by email.

You need to login to the secure Hosting Portal to review the credentials.

## 5. Accessing your CWP login

After clearing the SSL warning, you will see your server’s CWP login.

The first step is to configure your new site.

![](/assets/hosting/centos-web-panel.png)

Use the username/pass credentials provided in Statistics to sign in.

![](/assets/hosting/centos-web-panel-1.png)

Change or edit settings in the left menu navigation.

Access SSH terminal and file manager in top menu.

![](/assets/hosting/centos-web-panel-3.png)

## CentOS Web Panel tutorials

Find a CentOS Web Panel (CWP) developer on the HostJane Marketplace for consultation and help creating your new CWP site.

HostJane will support 24/7 server infrastructure and maintenance issues. However, CWP development / design is not offered by our support team.