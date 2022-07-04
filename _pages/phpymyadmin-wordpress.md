---
layout: default
title: phpMyAdmin on WordPress
parent: VPS Hosting
description: How to setup a WordPress VPS on HostJane
nav_order: 13
permalink: /vps-hosting/phpmyadmin-wordpress/
---

# Install phpMyAdmin on WordPress VPS

<span class="green">Access and make changes to your WordPress MySQL database.</span>

<span class="blue">[phpMyAdmin](https://www.phpmyadmin.net/) is a free database management tool.</span>

Because WordPress runs directly on the server, there isn’t a simple backend administrative interface where you can access phpMyAdmin as found in other software running WordPress (like cPanel).

Instead, phpMyAdmin must first be installed and then accessed via a standard browser window in Chrome or Firefox.

1. TOC
{:toc}

## 1. Download phpMyAdmin

[Latest version of phpMyAdmin](https://www.phpmyadmin.net/downloads/) can be downloaded as a zip file to your local computer.

Click the green download button or the .zip file on the top line of the phpMyAdmin latest releases.

## 2. FTP Login to your server

Connect with FileZilla

Use HostJane’s FTP tutorial to connect to your VPS.

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

You will be transferred to your WordPress server's dashboard. 

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

Below is a sample screenshot of the Server Information.

Below is a example screenshot of the Application Information.

| WordPress Server Details|
|:-------|
| To complete your WordPress installation follow these instructions: |
| 1. Log into the WP admin panel using the following credentials |
| `https://123.456.789.1/wp-admin` |
| `User: JaneDoe` |
| `Pass: 123456789` |
| Point your domain name "A record" to 123.456.789.1 |

### D. Open FileZilla

Enter the following information:

- [x] Host: sftp://[Your_Server’s_IP]
- [x] Username: root
- [x] Password: [Your_Server’s_Password] as found in Statistics
- [x] Port: 22

### E. Navigate to /var/www/html

Open /html folder:

![](/assets/hosting/ftp-var-www-html.png)

## 3. Upload phpMyAdmin to /html folder

In the left window, navigate to the phpMyAdmin .zip file you downloaded in Step 1.

Double-click it to upload it to your server’s /html folder.

![](/assets/hosting/upload-phpmyadmin.png)

View the uploaded document in the right-hand server window when the 10MB file upload completes:

![](/assets/hosting/server-window.png)

## 4. Unzip phpMyAdmin on the server

You cannot unzip files remotely using FTP.

<span class="green">Login to your server with PuTTY on Windows or an OpenSSH client in linux and MacOS devices to unzip the phpMyAdmin folder.</span>

After logging in, type this command to change directory to /html:

`cd /var/www/html`

Unzip the file:

`unzip phpMyAdmin-X.X.X-all-languages.zip`

Replace *phpMyAdmin-X.X.X-all-languages.zip* with the latest version phpMyAdmin of the one you downloaded.

**Press Enter**

You will see the phpMyAdmin zip being inflated into a directory folder on your  server, and stopping with a lint-query

![](/assets/hosting/inflating-phpmyadmin.png)

## 5. Change the phpMyAdmin directory name

To protect phpMyAdmin, change the directory name to your chosen name

In this tutorial, we will us: `janeadmin`

`mv phpMyAdmin-4.8.2-all-languages janeadmin`

Press Enter.

The cursor will move to the next line, and nothing will have appeared to have happened.

However, if you refresh your FileZilla window, you’ll see a new folder at the top of the tree, janeadmin.

This is visual confirmation the phpMyAdmin folder has been successfully changed.

![](/assets/hosting/janeadmin-folder-appears.png)

## 6. Create a configuration file for phpMyAdmin

Change the directory of your prompt user to janeadmin

`cd janeadmin`

Copy config.sample.inc.php and rename the copy to config.inc.php

`cp config.sample.inc.php config.inc.php`

Now open config.inc.php with nano, the command-line text editor.

`nano config.inc.php`

You will open the file with nano:

![](/assets/hosting/blowfish-secret.png)

Move the cursor to $cfg['blowfish_secret'] = '';

Enter a secret in the ” for blowfish_secret, for example:

`$cfg['blowfish_secret'] = 'janedoerocks-2837*2022o6)477sgrg';`

Use a random string of numbers, symbols, and letters of at least 32 characters and no more than 46 characters long for your blowfish secret

Write the changes with ctrl + O and press `Enter to save the changes`

Now exit back to the command line, with `ctrl + x`

## 7. Visit phpMyAdmin in the browser

Pull up a fresh browser window like Chrome, and enter into the address bar:

`https://[Your_Server’s_IP]/janeadmin`

![](/assets/hosting/phpmyadmin-browser.png)

## 8. Sign in to phpMyAdmin as root user

Make sure you are logged into the server (via OpenSSH or PuTTY) as the root user

### A. Obtain root password

To find out the root password to login to the phpMyAdmin management tool, enter on the CLI:

`cat /root/.my.cnf`

The phpMyAdmin root password will be displayed.

![](/assets/hosting/phpMyAdmin-password-mysql.png)

### B. Enter root credentials into browser:

<span class="purple">Username: root
Password: [As shown in the terminal shell]</span>

Proceed to enter phpMyAdmin

![](/assets/hosting/phpMyAdmin-logged-in.png)

## 9. Secure the phpMyAdmin installation

To ensure authorized users only can access phpMyAdmin in the browser, password secure the login.

![](/assets/hosting/security-phpmyadmin-shield.png)

In SSH, create an encrypted password by typing:

`openssl passwd`

For demo purposes, we used: *123456*

Don't use an easy password

Use a strong password generator to choose a secure, random password for your site.

Enter *123456*

The terminal returns an encrypted pass for `123456 of: Gc0VLaNLNhXoY`

![](/assets/hosting/security-phpmyadmin-passwd.png)

Go to the htpasswd directory:

`cd /etc/nginx/htpasswd/`

The  prompt will change to:

`root@host:/etc/nginx/htpasswd/$`

Using the nano command-line text editor to create a new file in the directory, such as *sizzler*

**Replace sizzler with your own username**

`nano sizzler`

The new file will open:

![](/assets/hosting/security-phpmyadmin-newfile.png)

Enter your credentials in the format: **Username : Encrypted pass**

In the above example, we input:

sizzler : Gc0VLaNLNhXoY

![](/assets/hosting/security-phpmyadmin-sizzler.png)

Write changes to the file with: ctrl + O and press Enter to save

Now exit with ctrl + x

Change directory again to:

`cd /etc/nginx/conf.d`

You need to nano edit 2 different (but very similar looking) files in this directory:

`wordpress_http.conf`
`wordpress_https.conf`

After changing to the /conf.d directory, first edit wordpress_http.conf

`nano wordpress_http.conf`

Find the line starting: 

`location ^~ /wp-admin/ {`

![](/assets/hosting/wordpress_http.conf_.png)

Change `/wp-admin/` to `/janeadmin/`

Next, move the cursor 2 lines down to find :

`auth_basic_user_file /etc/nginx/htpasswd/wp-admin;`

Change `/wp-admin/` to sizzler or the username you selected.

Write changes to the file with: ctrl + O and press Enter to save

Now exit with ctrl + x

The final result should look like:

![](/assets/hosting/changed-conf.png)

Now make the same edits to the second file: wordpress_https.conf

Finally, restart Nginx to apply changes:

`systemctl restart nginx`

Congratulations! You have now successfully set up a password screen to login to phpMyAdmin on your server.

In our above example, to login to phpMyAdmin at the security prompt::

`Username: sizzler (or your chosen username)
Password: 123456 (or your chosen password)`

phpMyAdmin is now safely behind locked doors for your use only.