---
layout: default
title: 1-Click WordPress
parent: VPS Hosting
description: How to setup a WordPress VPS on HostJane
nav_order: 2
permalink: /vps-hosting/wordpress-setup/
---

# WordPress Setup

<span class="blue">Setup a WordPress application on your server. Run themes and plugins from the WP ecosystem. Multisite is not currently supported. For server features, refer to the WordPress FAQ.</span>

1. TOC
{:toc}

## 1. Point your domain to the server

The first step is create an A-record at your domain registrar.
This enables you to access your server in any browser at your web domain.

Please note that it can take up to 72 hours for a domain to propagate throughout the internet to a server, although it usually happens much sooner.
We can’t set up your FREE SSL certificate until this step is completed.

## 2. Obtain your server’s details

### A. Login to the Hosting Portal

Bookmark login: https://console.hostjane.com/client/login

In your Dashboard under Services, find your WordPress server.

| Package | Label | Term  | Date Created | Date Renews | Options |
|:-------|:----------|:------|:----------|:------|:------|
| WordPress | Domain.com | 1 month @ $0.00 | Jan 1 | Feb 1 |*Manage* |

We offer 24×7×365 support

If you cannot see your WordPress service, open a support case.

### B. Click the Manage option

This is the button in the last column under Services.

Here is the next screen that will display: 

| Package | Status|
|:-------|:----------|
| WordPress | Active|
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

| WordPress Server Details|
|:-------|
| To complete your WordPress installation follow these instructions: |
| 1. log into the WP admin panel using the following credentials |
| `https://123.456.789.1/wp-admin` |
| `User: JaneDoe` |
| `Pass: 123456789` |

In this example, the server link is: https://123.456.789.1/wp-admin/

The first set of numbers before the /wp-admin/ is your server IP address.

In this example case the IP is: 123.456.789.1

<span class="red">Your Server Link
https://[Your_Server’s_IP]/wp-admin/</span>

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

## 4. Access the WordPress Installer

<span class="yellow">After passing the security dialog, you will see your server’s WordPress Installer for the latest version of WordPress.</span>

![](/assets/hosting/WordPress-installer-step1.png)

Click Continue

It’s a simple 2-step process.

All of the database credentials are already securely completed by HostJane for you.

You will need to enter:

1. Name of your site;
2. Your email
3. A new, unique username and password for your /wp-admin/ backend. 

#### Don't use an easy password

Use a strong password generator to choose a secure, random password for your site.

![](/assets/hosting/WordPress-installer-step2.png)

You will see a success message in the browser.

![](/assets/hosting/WordPress-installer-step3.png)

## 5. Login to WordPress

Login to your new site with the username and password you created in the previous step, and hit Login

![](/assets/hosting/WordPress-installer-step4.png)

You will then be forwarded to the WordPress Dashboard where you can manage your WordPress site.

![](/assets/hosting/WordPress-installer-step5.png)

## 6. Configure the WordPress URL

Your new site runs the latest version of WordPress.

Navigate to Settings > General Settings to enter YourDomain.com as the site title.

Replace your server IP address for the WordPress and Site URL.

![](/assets/hosting/Update-site-general-settings.png)

## WordPress tutorials

Find a WordPress developer on the HostJane Marketplace for consultation and help creating your new WordPress site.

HostJane will support 24/7 server infrastructure and maintenance issues. However, WordPress development / design is not offered by our support team.

---

# WordPress VPS FAQ

## How can I access WordPress files without cPanel (or another CMS?

1. You will need to either use FTP to change files in your WordPress installation, or install a back-end file manager plugin.

2. We run WordPress directly on the server. Apart from the WordPress dashboard it doesn't include a server administration platform like cPanel/WHM or Plesk.

## WordPress plugins disallowed on JaneVPS
Unlike other WordPress-specialty hosts that ban their users from installing certain plugins, we're not code snobs about what software you can and can't use on your own website.
However if we believe there is software on your server that could potentially cause security issues on the network, we'll contact you.

## Choose your plugins carefully

We advise WordPress VPS customers to have a very careful read of available information on the WordPress plugins repository before installing any particular plugin on their WordPress site.

Give preference to plugins with a developer who is easy to contact and updates his or her plugin on a regular basis

1. Look for a 'Last Updated' dateline within the last 1-3 months;
2. Over 5,000+ current uses;
3. Up-to-date WP version compatibility;
4. Good reviews 

Plugins that are top-heavy with genuine bad reviews, including complaints about security flaws we would advise you to proceed with caution.

![](/assets/hosting/wp-plugin-versions.png)

Always try to use the most up-to-date versions of plugins and themes at all times, and keep WordPress up-to-date. At the end of the day, it's your VPS so as long as you are abiding by HostJane's AUP and TOS, you can do what you like.

## How do I set up my WordPress VPS?

Please follow [t]hese instructions](/vps-hosting/point-your-domain/) to set up your WordPress server.

The first step is to point your domain to the server at your domain registrar by creating an A-record.

Important: An SSL browser warning appears during normal set up when you access your WordPress /wp-admin/ backend using HTTPS://

This is normal and disappears when SSL is installed.

## Migrating your WordPress site

Read our WordPress Migration guide

We recommend ServMask, Inc's All-in-one WP Migration plugin which reliably transfers most WordPress sites in a few clicks.

## How secure is HostJane VPS?

In short, extremely secure with multiple layers of physical and cyber protection.

Your server is held in a private Tier III datacenter which undergoes:

- [x] Regular audits
- [x] Strict authorized access monitored by CCTV
- [x] Retinal and fingerprint scans
- [x] 24/7/365 on-site security.

The facilities are also protected against flooding and fire, and backups are stored at different locations.

On the virtual level, both the datacenter and HostJane are continuously monitoring for suspicious activity and updating to guard against malicious cyber attacks.

## Does WordPress VPS offer staging sites?

We offer a privacy feature where only the IP addresses you approve will have access to your VPS. 

Open a support case to add or remove IP addresses from your private whitelist.

## Does WordPress VPS use Apache?

No, WordPress VPS uses the latest Ubuntu version with NGINX in its web server layer.

The latest versions of PHP and MySQL are installed in the LEMP stack.

## Is IPv6 support included?

Yes, you can choose to set up your WordPress VPS with an IPv6 address at checkout.

A dedicated IPv4 address is included with each plan.

## How do I access my database?

We recommend phpMyAdmin to manage your wordpress MySQL databases.

Install phpMyAdmin with this WordPress VPS tutorial on phpMyAdmin

## Do you offer multisite?

No. Each WordPress VPS plan provides for a single, regular WordPress site installation that connects to 1 domain only.