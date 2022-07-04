---
layout: default
title: 1-Click cPanel/WHM
parent: VPS Hosting
description: How to setup a WordPress VPS on HostJane
nav_order: 3
permalink: /vps-hosting/cpanel-whm-vps/
---

# cPanel/WHM Set-up

HostJane cPanel VPS comes pre-installed with cPanel/WHM on a managed server running Centos 7 x64. For more technical details of the server, refer to Server FAQ.

A server with at least 2GB RAM is required.

1. TOC
{:toc}

#### License Pricing

<span class="purple">cPanel is licensed based on the number of accounts used in the application. Select the tier of accounts needed starting from 1 to 5 through to 500-1000 during VPS checkout.</span>

## 1. Point your domain to the server
The first step is create an A-record at your domain registrar.
This enables you to access your server in any browser at your web domain.

Please note that it can take up to 72 hours for a domain to propagate throughout the internet to a server, although it usually happens much sooner.

We can’t set up your FREE SSL certificate until this step is completed.

## 2. Obtain your server’s details

### A. Login to the Hosting Portal

Bookmark login: https://console.hostjane.com/client/login

In your Dashboard under Services, find your cPanel/WHM server.

We offer 24×7×365 support

| Package | Label | Term  | Date Created | Date Renews | Options |
|:-------|:----------|:------|:----------|:------|:------|
| cPanel | Domain.com | 1 month @ $0.00 | Jan 1 | Feb 1 |*Manage* |

If you cannot see your WordPress service, open a support case.

### B. Click the Manage option

This is the button in the last column under Services.

Here is the next screen that will display: 

| Package | Status|
|:-------|:----------|
| cPanel | Active|
| **Label** | **Renew Date**|
| Domain.com | Feb 1 |
| **Creation Date** | **Next Invoice**|
| Jan 1 | Feb 1 |
| **Billing Cycle** | **Recurring Amount**|
| 1 Month | $0.00 |

### C. Click Statistics in the menu

Your private and confidential server root password and IP address is in Statistics.

Security Alert

Never disclose, email, or publish your password to anyone, including HostJane staff in support tickets. Our technicians have safe access inside secure datacenters if they need this.

Below is a example screenshot of the Application Information.

| WordPress Server Details|
|:-------|
| To complete your WordPress installation follow these instructions: |
| 1. log into the WP admin panel using the following credentials |
| `https://123.456.789.1/2087` |
| `User: root` |
| `Pass: 123456789` |

In this example, the server link is: https://123.456.789.1:2087/

The first set of numbers before the :2087/ is your server IP address.

In this example case the IP is: 123.456.789.1

<span class="yellow">Your Server Link
https://[Your_Server’s_IP]:2087/</span>

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

## 4. Access the cPanel Installer

After ignoring the SSL warning, you will find your server’s cPanel Installer page.

![](/assets/hosting/cpanel-1.png)

This will install the latest version of cPanel/WHM.

Bookmark your server link

You will only have to go through this installer once.

After cPanel/WHM is configured, and you have created at least ONE (1) cPanel account, you can access your cPanel/WHM server via this URL:

<span class="green">https://[Your_Server’s_IP]:2083/</span>

Replace your actual server's IP with [_Your_Server's_IP] in the above link.

## 5. Agree to the cPanel/WHM license

You'll need to read and agree to the terms of the cPanel license to proceed.

![](/assets/hosting/cpanel-WHM-Agree-to-license.png)

## 6. Setup your global email
This is done through the Networking page. Make sure this is a reliable email which you have access to.

![](/assets/hosting/cpanel-WHM-Setup-networking-email.png)

## 7. Setup the Networking page

After entering your email, scroll down and clear out the cpanel171938…. information.

![](/assets/hosting/cpanel-WHM-Setup-networking-hostname.png)

Replace it with your own Fully-Qualified Domain Name (FQDN).

<span class="yellow">A FQDN is, for example, Host.YourDomain.com</span>

![](/assets/hosting/cpanel-WHM-Setup-networking-hostname-FQDN.png)

### What is a Fully-Qualified Domain Name?

A Fully-Qualified Domain Name is a phrase geeks use to talk about the exact location of your domain name inside the Domain Name System (DNS). It's the complete description of a computer, or host, on the internet.

Your FQDN is made of 2 parts:

1. Your domain name. This includes the Top-level domain (TLD). In this case, YourDomain.com
2. The hostname. This can be host, www, mail or any other word. In this case, it's Host in: Host.YourDomain.com

### Setup the Resolvers

In the bottom section of the Networking page, set the primary and secondary name resolvers.

![](/assets/hosting/cpanel-WHM-Setup-networking-resolvers.png)

We recommend using Google’s Public DNS IP address: 8.8.8.8, as the secondary resolver.

## 8. Skip Set Up IP Addresses

Unless you know what you’re doing, we recommend you leave the next step section about IP addresses for now.

![](/assets/hosting/cpanel-WHM-Setup-IP-Addresses.png)

## 9. Setup your Nameservers

Ensure Bind is checked.

![](/assets/hosting/cpanel-WHM-Setup-NameServers-BIND.png)

You will need to set up your nameservers.

Recommended settings
NS1.YourDomain.com
NS2.YourDomain.com

![](/assets/hosting/cpanel-WHM-Setup-NameServers-NS1-NS2.png)

If you intend to point multiple domains at the server, you will need to configure your nameservers at the domain registrar.

This will require you to obtain a second IP address for the second NS2 nameserver.

## Purchasing additional IP addresses

Open a support ticket if you wish to buy a second IP address from HostJane for this purpose. We charge $4 per month per IP address which may be subject to IP justification.

Unless you know what you’re doing, do not change the bottom section that should display your server’s IP address.

![](/assets/hosting/cpanel-WHM-Setup-NameServers-A-RECORD.png)

Click Save and Go to Step 5

## 10. Skip Services

We recommend skipping the Services section, unless you know what you're doing.

![](/assets/hosting/cpanel-WHM-Setup-cpanel-Services.png)

Click Save and Go to Step 6

## 11. Allow filesystem quotas

![](/assets/hosting/cpanel-WHM-Setup-cpanel-quotas.png)

Click Finish

## 12. Complete the installer

We recommend you clear any prompts about your server’s memory limits by clicking Go to WHM

![](/assets/hosting/cpanel-WHM-Setup-cpanel-beforeyougo.png)

## 13. Feature Showcase

Choose the features you would prefer, then at the bottom of the Feature Showcase, click Save Settings

![](/assets/hosting/cpanel-WHM-Setup-cpanel-feature-showcase.png)

## 14. Setup a New Account

Within the cPanel/WHM dashboard, navigate to Account Functions > Create a New Account

You need to create an account for your primary domain, YourDomain.com. This is the domain you are pointing at the server with an A-record. 

![](/assets/hosting/cpanel-WHM-Setup-cpanel-feature-createanew-account.png)

Enter YourDomain.com

Choose a username and password, and click Create

Depending on your configuration, you will be managing your DNS records either locally on your server or at your domain registrar.

## 15. Access Your Domain's cPanel account

Navigate to Account Information > List Accounts to access YourDomain.com’s cPanel account.

![](/assets/hosting/list-accounts-cpanel-whm.png)

Click the orange cPanel button.

YourDomain.com’s account will open in a new window and you can begin to build your site.

Be aware you will be accessing your cPanel with root access.

## Building your site

Files you add to the public_html folder will be accessible at YourDomain.com/[name_of_file]

Using multiple domains with your server

1) Obtain a second IP address from either HostJane at $4 per month or somewhere else.

2) Associate the IP addresses with custom nameservers at your domain registrar.

#### Example DNS setup

NS1.YourDomain.com –> Main Server IP Address

NS2.YourDomain.com –> Second IP Address

3) Navigate to Server Configuration > Basic WebHost Manager® Setup

![](/assets/hosting/basic-webhost-manager-setup.png)

At the bottom of the WebHost Manager Setup, configure your 2 nameservers with the 2 IP addresses.

4) Ensure each new domain that points to your server is set up at each registrar with the same custom nameservers:

In our example case:

NS1.YourDomain.com –> Main Server IP Address

NS2.YourDomain.com –> Second IP Address

### cPanel/WHM tutorials

Find a cPanel developer on the HostJane Marketplace for consultation and help creating your new WordPress site.

HostJane will support 24/7 server infrastructure and maintenance issues. However, WordPress development / design is not offered by our support team.