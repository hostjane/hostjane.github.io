---
layout: default
title: 1-Click MediaWiki
parent: VPS Hosting
description: How to setup a MediaWiki VPS on HostJane
nav_order: 12
permalink: /vps-hosting/mediawiki/
---

# 1-Click MediaWiki
{: .no_toc }

<span class="green">Setup a MediaWiki application on your server. For more technical details about HostJane servers, read [our FAQ](/vps-hosting).</span>

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

In your Dashboard under Services, find your MediaWiki server.

| Package | Label | Term  | Date Created | Date Renews | Options |
|:-------|:----------|:------|:----------|:------|:------|
| MediaWiki | Domain.com | 1 month @ $0.00 | Jan 1 | Feb 1 |*Manage* |

We offer 24×7×365 support

If you cannot see your WordPress service, open a support case.

### B. Click the Manage option

This is the button in the last column under Services.

Here is the next screen that will display: 

| Package | Status|
|:-------|:----------|
| MediaWiki | Active|
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

| MediaWiki Server Details|
|:-------|
| Complete your MediaWiki installation by accessing this URL: |
| `https://123.456.789.1/mw-config/` |
| The installer will prompt you for login credentials and an upgrade key |
| You will need these credentials to access the installer |
| Login user: demo |
| Login pass: demo123 |
| When the installer reads "...please enter the valye of $wgUpgradeKey in the box below...", you will need this upgrade key: |
| Upgrade key: `demokey` |

In this example, the server link is: https://123.456.789.1/mw-config/

The first set of numbers before the /mw-config/ is your server IP address.

In this example case the IP is: 123.456.789.1

Your Server Link
https://[Your_Server’s_IP]/mw-config/
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

## 4. Access the MediaWiki Installer

After passing the security dialog, you will see your server’s MediaWiki Installer.

The first step is to configure your new site.

![](/assets/hosting/media-wiki-installer.png)

Configure your upgrade key

![](/assets/hosting/media-wiki-upgradekey.png)

Copy and paste the upgrade key as provided in Statistics.

| When the installer reads "...please enter the valye of $wgUpgradeKey in the box below...", you will need this upgrade key: |
| Upgrade key: `demokey` |

<span class="red">The key must match exactly.</span>

Click continue to move through the environmental checks

![](/assets/hosting/media-wiki-environmental-checks.png)

Click continue

Leave the database settings with Use same account as for installation checked.

![](/assets/hosting/media-wiki-database-settings-install.png)

Click continue

Create the username and password details for your MediaWiki’s administrator account

Don't use an easy password

Use a strong password generator to choose a secure, random password for your site. 

![](/assets/hosting/media-wiki-site-set-up.png)

We do not recommend clicking “I’m bored, set up the wiki”.

Click continue

The Options setup page is an important step.

You can control:

1. How much access new users have on your Wiki site
2. Copyright licensing
3. Set up skins
4. Advanced functions.

![](/assets/hosting/media-wiki-site-options.png)

When you have selected your configuration, click continue to begin installation.

![](/assets/hosting/media-wiki-start-installation.png)

Click continue

![](/assets/hosting/media-wiki-successful-completion.png)

The installation is now complete!

 You can IGNORE the final instruction requiring you to download and install the localsettings.php file in the base directory

![](/assets/hosting/media-wiki-final-stage.png)

## 5. Access your MediaWiki site

Once your domain has finished pointing to the server, you will be able to access your website via your domain name.

![](/assets/hosting/media-wiki-front-end.png)

## MediaWiki Help

Find a MediaWiki developer on the HostJane Marketplace for consultation and help creating your new MediaWiki site.

HostJane will support 24/7 server infrastructure and maintenance issues. However, MediaWiki development / design is not offered by our support team.