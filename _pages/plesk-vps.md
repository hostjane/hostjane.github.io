---
layout: default
title: 1-Click Plesk
parent: VPS Hosting
description: How to setup a Plesk VPS on HostJane
nav_order: 10
permalink: /vps-hosting/plesk-vps/
---

# 1-Click Plesk
{: .no_toc }

<span class="green">Setup a Plesk application on your server. Plesk is available in 3 different editions–Web Admin, Web Pro and Web Host. Plesk provide a comparison guide to assist in choosing the appropriate version for your needs.</span>

## In this section
{: .no_toc .text-delta }

1. TOC
{:toc}

## 1. Point your domain to the server

The first step is create an A-record at your domain registrar.
This enables you to access your server in any browser at your web domain.

<span class="blue">Please note that it can take up to 72 hours for a domain to propagate throughout the internet to a server, although it usually happens much sooner.</span>

We can’t set up your FREE SSL certificate until this step is completed.

## 2. Obtain your server’s details

### A. Login to the Hosting Portal

Bookmark login: https://console.hostjane.com/client/login

In your Dashboard under Services, find your Plesk server.

| Package | Label | Term  | Date Created | Date Renews | Options |
|:-------|:----------|:------|:----------|:------|:------|
| Plesk | Domain.com | 1 month @ $0.00 | Jan 1 | Feb 1 |*Manage* |

We offer 24×7×365 support

If you cannot see your Plesk service, open a support case.

### B. Click the Manage option

This is the button in the last column under Services.

Here is the next screen that will display: 

| Package | Status|
|:-------|:----------|
| Plesk | Active|
| **Label** | **Renew Date**|
| Domain.com | Feb 1 |
| **Creation Date** | **Next Invoice**|
| Jan 1 | Feb 1 |
| **Billing Cycle** | **Recurring Amount**|
| 1 Month | $0.00 |

### C. Click Statistics in the menu

Your private and confidential server root password and IP address is in *Statistics*.

#### Security Alert

<span class="green">Never disclose, email, or publish your password to anyone, including HostJane staff in support tickets. Our technicians have safe access inside secure datacenters if they need this.</span>

Below is a example screenshot of the Application Information.

### D. Click Manage next to the Plesk server item

You will be transferred to the server’s dashboard.

### E. Go to the Statistics area

Find your server’s IP address and password.

Follow the instructions to complete your Plesk installation.

Sample screenshot of the Application Information.

| Plesk Onyx Server Details|
|:-------|
| Your Plesk Onyx server will reboot once after the initial deployment |
| Access your Plesk Onyx server by visiting this URL: |
| `https://123.456.789.1:8443/login` |
| Login user: root |
| Login pass: Example1234 |
| Your Plesk Onyx app activates automatically when it is first deployed. If you are prompted for an activation code, you may use the following one. |
| Activation code: AAAAAA-BBBBBB-CCCCCC-DDDDDD-EEEEEE |


In this example, the server link is: https://123.456.789.1:8443/login

The first set of numbers before the :8443/login is your server IP address.

In this example case the IP is: 123.456.789.1

Your Server Link
https://[Your_Server’s_IP]:8443/login

For security, HostJane does not send this to you by email.

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

## 4. Login to Plesk server

After passing the security dialog, you will see your server’s Plesk login page.

![](/assets/hosting/plesk-login-backend.png)

You need to login with username: root and the root password given in Statistics

## 5. Activation Code

Your plesk server should be activated automatically, but if you are prompted to enter an Activation Code, this is available in Statistics

<span class="yellow">Find the long Activate Code in the format: AAAAAA-BBBBBB-CCCCCC-DDDDDD-EEEEEE</span>

*Proceed to Login*

Replace your Your Contact Name and Email with your own details.

Plesk initializing screen appears

![](/assets/hosting/plesk-setup-intializing.png)

Now you can setup your Plesk dashboard

![](/assets/hosting/plesk-setup-dashboard.png)

## 6. Configure Plesk Hostname

Once your domain has finished pointing to the server, you will be able to access your Plesk front-end in the browser via YourDomainName.TLD

Navigate to:

Server Management > Tools & Settings > Server Settings to update your domain name (hostname).

## 7. Add New Domain Name

Inside your Plesk dashboard:

Navigate to:

Hosting Services > Domains > Add New Domain to configure your domain name (hostname).

![](/assets/hosting/plesk-domain-setup.png)

Check the option in the domain setup to install your free SSL certificate from Let’s Encrypt, a San Francisco-based provider of free SSL certificates sponsored by Mozilla Firefox and Google Chrome.

Your installation is now complete!

## Plesk Advanced Help

Find a Plesk developer on the HostJane Marketplace for consultation and help creating your new Plesk site.

HostJane will support 24/7 server infrastructure and maintenance issues. However, Plesk development / design is not offered by our support team.