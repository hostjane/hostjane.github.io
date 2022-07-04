---
layout: default
title: 1-Click PrestaShop
parent: VPS Hosting
description: How to setup a WordPress VPS on HostJane
nav_order: 6
permalink: /vps-hosting/prestashop/
---

Setup a PrestaShop application on server. Note that PrestaShop does require you to modify 1 file via Secure Shell (SSH) client to complete installation.
Step-by-Step Instructions
1. Point your domain to the server
The first step is create an A-record at your domain registrar.
This enables you to access your server in any browser at your web domain.

Please note that it can take up to 72 hours for a domain to propagate throughout the internet to a server, although it usually happens much sooner.
We can’t set up your FREE SSL certificate until this step is completed.

2. Obtain your server’s details
A. Login to the Hosting Portal
Bookmark login: https://console.hostjane.com/client/login

In your Dashboard under Services, find your PrestaShop server.


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


In this example, the server link is: https://123.456.789.1/install/

The first set of numbers before the /install/ is your server IP address.

In this example case the IP is: 123.456.789.1

Your Server Link
https://[Your_Server’s_IP]/install/
The PrestaShop database will also require configuring during the install process.

The username and passwords for the database are found in Statistics.

Yours will look something like the image below:


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

4. Access the PrestaShop Installer
After passing the security dialog, you will see your server’s PrestaShop Installer.

The first step is to configure your new site.


Click Next

Agree to the licensing terms and click Next


At the compatibility prompt, click Next


Configure your store’s login, category, and account information, then click Next

Don't use an easy password
Use a strong password generator to choose a secure, random password for your site.

Locate your server’s database credentials in Statistics and complete the database configuration for your PrestaShop server.


Fields that are not mentioned in statistics do NOT need to be changed.


Click Test your database connection now and a green box should appear indicating a successful connection.

Double check your credentials
Ensure you have entered your database username and password details correctly from Statistics if you do not see this button.


Click Next
There will be a short wait while the installation completes.


The installation will complete, reminding you of the login information you selected.


5. Modify installation by SSH
Before you try to access your PrestaShop installation in the browser, you must remove the /install folder for security reasons.

This can only be removed by using a Secure Shell client.

You need to login to your server with the root username.

ssh root@[Your_Server’s_IP]

Login by SSH
Use the information from Statistics to login either with PuTTY on Windows or an OpenSSH client in linux and MacOS devices.


Inside your server’s dashboard under Statistics:

Your PrestaShop server’s IP address is shown as Main IP (see red arrows above).
Your server’s root password is the Default Password
Walkthrough with PuTTY for Windows users
Remove the /install folder using any SSH client such as PuTTY.

Download and install PuTTY from the official website.


Once it’s installed, open PuTTY and type your PrestaShop server IP address as given in Statistics

Ensure the Port is 22 and click Open

Click Yes at the security prompt.


Proceed to enter root as the login name

Click Enter

Enter your password as given in Statistics

Case-sensitive requirement
Your password is a long string of lowercase, uppercase letters, and symbols. Enter it exactly. For security reasons, the cursor does not move when you enter a password on the command line.

Once you have successfully logged in, you will see the Ubuntu welcome screen:



Enter this line

rm -rf /var/www/html/install
Hit Enter

Exit the Putty by closing the dialog and closing the session at the prompt, or by type Exit and hit Enter.

6. Test the installation
If you successfully removed the /install folder, you will be able to login to your new PrestaShop store in your browser with the following URLs:

Admin area: https://[Your_Server’s_IP]/admin_area/

Store: https://[Your_Server’s_IP]

If you are prompted again by a security dialog, enter the username and password for the server from Statistics.


The PrestaShop backend should then load in your browser:


Enter the username and password you selected during the PrestaShop installer to log in:


The front-end will show with installed sample data:


Your PrestaShop installation is now complete!

Advanced PrestaShop Setup
Find a PrestaShop developer on the HostJane Marketplace for consultation and help creating your new PrestaShop site.
HostJane will support 24/7 server infrastructure and maintenance issues. However, PrestaShop development / design is not offered by our support team.