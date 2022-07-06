---
layout: default
title: 1-Click Joomla
parent: VPS Hosting
description: How to setup a Joomla VPS on HostJane
nav_order: 4
permalink: /vps-hosting/joomla/
---

# 1-Click Joomla

<span class="yellow">Setup a Joomla application on your server. Read our VPS Features for more information about your server.</span>

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

In your Dashboard under Services, find your Joomla server.

| Package | Label | Term  | Date Created | Date Renews | Options |
|:-------|:----------|:------|:----------|:------|:------|
| Joomla | Domain.com | 1 month @ $0.00 | Jan 1 | Feb 1 |*Manage* |

We offer 24×7×365 support

If you cannot see your WordPress service, open a support case.

### B. Click the Manage option

This is the button in the last column under Services.

Here is the next screen that will display: 

| Package | Status|
|:-------|:----------|
| Joomla | Active|
| **Label** | **Renew Date**|
| Domain.com | Feb 1 |
| **Creation Date** | **Next Invoice**|
| Jan 1 | Feb 1 |
| **Billing Cycle** | **Recurring Amount**|
| 1 Month | $0.00 |


### C. Click Statistics in the menu

Your private and confidential server root password and IP address is in *Statistics*.

#### Security Alert

<span class="blue">Never disclose, email, or publish your password to anyone, including HostJane staff in support tickets. Our technicians have safe access inside secure datacenters if they need this.</span>

Below is an **example** screenshot of the Application Information.

| Joomla Server Details|
|:-------|
| Complete your Joomla installation by accessig this URL: |
| https://123.456.789.1/installation/ |
| The installer will prompt you for login credentials and local database settings. |
| You will need these credentials to access the installer: |
| `Login user: JaneDoe` |
| `Login pass: 123456789` |
| On the "Database Configuration" step, update the fields on the page with the values below. Fields that are not mentioned do not need to be changed. |
| Database Type: MySQLi |
| Username: Janeuser |
| Password: Example1 |
| Database Name: Database Name |
| After you finish the installation, you Joomla website will be accessible at: |
| https://123.456.789.1/ |

In this example, the server link is: https://123.456.789.1/installation/

The first set of numbers before the /installation/ is your server IP address.

In this example case the IP is: 123.456.789.1

```
Your Server Link
https://[Your_Server’s_IP]/installation/
```

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

## 4. Accessing the Joomla Installer

After passing the security dialog, you will see your server's Joomla Installer.

The first step is to configure your new site.

![](/assets/hosting/joomla-installation-step-1.png)

The next step is to configure your Joomla Database.

Complete the database user/pass credentials by copying and pasting the information provided in Statistics as shown above.

The details must match exactly. Unless you know what you’re doing:

- Leave the Database Type as: `MySQli`
- Leave the Host Name as: `Local Host`

**Don't use an easy password**

Use a strong password generator to choose a secure, random password for your site.

![](/assets/hosting/joomla-installation-step-2-database.png)

Click Next to move to the final step

Select whether you wish to install Joomla’s Sample Data which decides whether you want the first version of your site to be published blank or with example texts and modules applied.

![](/assets/hosting/joomla-installation-step-3-finalizing-data.png)

Check the details are correct under Main Configuration and Database Configuration at the bottom, then click Install

![](/assets/hosting/joomla-installation-step-3-check-details.png)

The installer should complete successfully.

![](/assets/hosting/joomla-installation-step-4-installer-completed.png)

Your Joomla installation is now complete.

## 5. Secure the installation

It’s important to click the Remove “Installation” folder button on this page to secure your new Joomla site from common exploits.

The button should change to “Installation” folder removed to confirm this.

![](/assets/hosting/site-administrator-buttons-joomla.png)

Click the 2 buttons Site and Administrator to view the front and backends of your new Joomla site in the browser.

## 6. Login to Joomla

The front-end will look like the below image in your browser (With no Sample Data installed)

![](/assets/hosting/joomla-front-end-browser.png)

The back-end will look like below, you may be prompted to update if a more recent Joomla version is available.

![](/assets/hosting/joomla-back-end-browser.png)

## Joomla Design / Development

Find a Joomla developer on the HostJane Marketplace for consultation and help creating your new Joomla site.

HostJane will support 24/7 server infrastructure and maintenance issues. However, Joomla development / design is not offered by our support team