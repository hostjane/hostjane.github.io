---
layout: default
title: 1-Click GitLab
parent: Cloud Computes
description: How to setup a LAMP server
nav_order: 9
permalink: /cloud-compute/gitlab/
---

Tutorial for running latest GitLab version on HostJane.
HostJane’s cloud servers runs the GitLab Community Edition (CE) on Ubuntu. 
Note that GitLab requires a cloud compute running at the minimum 2 CPU.
1. Get server IP and root password
After successful payment is approved, your server will be set up within usually 2 minutes.
A. Login to the Hosting Portal
Bookmark login: https://console.hostjane.com/client/login

In the Dashboard under Services, look for the GitLab server you have provisioned.



We offer 24×7×365 support
If you cannot see your service, open a support case.

B. Click Manage next to the GitLab server item
You will be transferred to the server’s dashboard.



C. Click Statistics in the menu
Below is a sample screenshot of the Server Information.



In this example, the server link is: https://123.456.789.1:
In this example case the IP is: 123.456.789.1

Your Server Link
https://[Your_Server’s_IP]/
For security, HostJane does not send this to you by email.

You must login to your hosting account to review these credentials.

2. Ignore the browser warning
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

3. Access the Gitlab installer
After passing the security dialog, you will see your server’s GitLab signin.



Copy and paste the root username and password as provided in Statistics to login to your GitLab portal:



4. Update your domain URL to GitLab configuration
It’s not enough to simply point your domain to your GitLab server, you need to ensure that clone URLs are not generated that could impede your workflow.

Login to your server with PuTTY on Windows or an OpenSSH client in linux and MacOS devices:
ssh -l root [Your_Server's_IP]
Once logged in as the root user, use the nano command-line text editor to edit the following file:

nano /etc/gitlab/gitlab.rb

Move the cursor to change the external_url from:

external_url https://[Your_Server's_IP]
Change to your domain:

external_url https://YourDomain.com
Press ctrl + O then Enter to write the changes to SSH daemon

Now close the file with ctrl + x

Reconfigure the GitLab server by typing:

gitlab-ctl reconfigure
You have successfully installed your Gitlab server!

All repositories created and managed through the GUI can be found located at:

/var/opt/gitlab/git-data/repositories
