---
layout: default
title: 1-Click Drupal
parent: VPS Hosting
description: How to setup a WordPress VPS on HostJane
nav_order: 11
permalink: /vps-hosting/drupal-vps/
---

Install a Drupal application uses Ubuntu in a LEMP stack. Note your server is running NGINX in its web server stack.
Step-by-Step Instructions
1. Point your domain to the server
The first step is create an A-record at your domain registrar.
This enables you to access your server in any browser at your web domain.

Please note that it can take up to 72 hours for a domain to propagate throughout the internet to a server, although it usually happens much sooner.
We can’t set up your FREE SSL certificate until this step is completed.

2. Obtain your server’s details
A. Login to the Hosting Portal
Bookmark login: https://console.hostjane.com/client/login

In your Dashboard under Services, find your Drupal server.



We offer 24×7×365 support
If you cannot see your WordPress service, open a support case.

B. Click the Manage option
This is the button in the last column under Services.

Here is the next screen that will display: 


C. Click Statistics in the menu
Your private and confidential server root password and IP address is in Statistics.

Security Alert
Never disclose, email, or publish your password to anyone, including HostJane staff in support tickets. Our technicians have safe access inside secure datacenters if they need this.
Below is a example screenshot of the Application Information.


In this example, the server link is: https://123.456.789.1/install.php

The first set of numbers before the /install.php is your server IP address.

In this example case the IP is: 123.456.789.1

Your Server Link
https://[Your_Server’s_IP]/install.php
For security, HostJane does not send this to you by email.

You must login to your hosting account to review these credentials.

3. Ignore the browser warning
A. Copy and paste your unique server link 
Open a fresh browser window and paste the link

Hit Enter.

B. Find the HTTPS warning
The warning can be safely ignored.
It will look slightly different depending on which browse you're using. In Chrome it may appear like this:



In Mozilla Firefox, it may look like this:



Click the Advanced or Add Exception link to accept the warning and proceed to the unsafe page.

A security dialog box will open.



Enter the username and password credentials into the box, as found in Statistics.

Click Sign in or Enter.

Why is there a warning?
HostJane cannot configure an SSL certificate (HTTPS://) for an IP address on its own. We need to wait until your domain is pointing to the server, and then assign your FREE SSL certificate to your domain.
Until your domain's A-record is setup, whenever you access your server by HTTPS://, a warning appears in your browser.

Your server comes with a self-signed SSL certificate.

If you access the server link using HTTP://, you will not see the warning. 

C. How to remove the SSL warning
Once your domain's A-record is successfully pointing to your server, HostJane can install your FREE SSL certificate to remove the warning.

Request your FREE SSL certificate
Open a support ticket after your domain is pointed correctly to your server.
You can check when propagation is successful by doing a DNS lookup of your domain's A-record.
Please note that we can only install an SSL certificate on a top-level domain (TLD)
For example: https://www.yourdomain.TLD, where the TLD could be .com, .net, .org, .ca, or any TLD available.

HostJane and our servers work with all domain registrars worldwide.

4. Accessing the Drupal Installer
After passing the security dialog, you will see your server’s Drupal Installer for the latest version of Drupal.



Follow the on-screen steps, reviewing the Drupal set up information.

Hit the browser back button if you need to return to the previous menu.



Most people opt for the standard installation.



Complete the database user/pass credentials by copying and pasting the information provided in Statistics as shown above.

The installer will then initialize.


This takes less than 30 seconds to install Drupal’s modules and framework.


You will finally come to the Configure Site screen, where you will:

Name your site
Enter a global email for the site
Choose a username
Choose a password
Complete regional settings
Choose your notification preferences
Don't use an easy password
Use a strong password generator to choose a secure, random password for your site.



Upon Saving the details, you will be forwarded to the homepage of your site.

5. Login to Drupal
To access the Drupal administration portal, before your domain successfully propagates, use:

https://[Your_Server’s_IP]/admin

After propagation is complete, use: https://www.YourDomain.com/admin


After logging in, you will see the Drupal dashboard.



Your Drupal installation is now complete.

Drupal Design / Development
Find a Drupal developer on the HostJane Marketplace for consultation and help creating your new Drupal site.
HostJane will support 24/7 server infrastructure and maintenance issues. However, Drupal development / design is not offered by our support team.