---
layout: default
title: 1-Click OpenVPN
parent: Cloud Computes
description: How to setup an OpenVPN server
nav_order: 9
permalink: /cloud-compute/openvpn/
---

# 1-Click OpenVPN

<span class="yellow">HostJane runs OpenVPN on Ubuntu, one of the most secure linux distributions. OpenVPN on HostJane Cloud only allows two (2) devices to connect free at any 1 time.</span>

If you need to connect more devices, then you need to buy a license from OpenVPN.

1. TOC
{:toc}

## 1. Get server IP and root password

After successful payment is approved, your server will be set up within 2 minutes.

### A. Login to the Hosting Portal

Bookmark login: [https://console.hostjane.com/client/login](https://console.hostjane.com/client/login)

In your Dashboard under Services, find your OpenVPN server.

| Package | Label | Term  | Date Created | Date Renews | Options |
|:-------|:----------|:------|:----------|:------|:------|
| OpenVPN | host.domain.com | 1 month @ $0.00 | Jan 1 | Feb 1 |*Manage* |

We offer 24×7×365 support

If you cannot see your OpenVPN service, open a support case.

### B. Click the Manage option

This is the button in the last column under Services.

Here is the next screen that will display: 

| Package | Status|
|:-------|:----------|
| OpenVPN | Active|
| **Label** | **Renew Date**|
| host.domain.com | Feb 1 |
| **Creation Date** | **Next Invoice**|
| Jan 1 | Feb 1 |
| **Billing Cycle** | **Recurring Amount**|
| 1 Month | $0.00 |

### C. Click Statistics in the menu

Below is a sample screenshot of the Server Information.

| OpenVPN Server Details |
| Complete your OpenVPN installation by visiting this URL: |
| https://123.456.789.1/ |
| User: openvpn |
| Pass: demo |

In this example, the server link is: https://123.456.789.1

In this example case the IP is: 123.456.789.1

```
Your Server Link
https://[Your_Server’s_IP]/
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

1. Open a support ticket after your domain is pointed correctly to your server.
2. You can check when propagation is successful by doing a DNS lookup of your domain's A-record.
3. Please note that we can only install an SSL certificate on a top-level domain (TLD)

For example: https://www.yourdomain.TLD, where the TLD could be .com, .net, .org, .ca, or any TLD available.

HostJane and our servers work with all domain registrars worldwide.

## 3. Access the OpenVPN installer

After passing the security dialog, you will see the OpenVPN login page.

![](\assets\hosting\openvpn-login.png)

Enter the username and password given in Statistics

![](\assets\hosting\openvpn-options.png)

You can now download the OpenVPN client for your system, to connect to OpenVPN.

To proceed with OpenVPN configuration, click Admin

Enter the username and password given in Statistics.

![](\assets\hosting\openvpn-admin.png)

Agree to the terms of use.

![](\assets\hosting\openvpn-admin-logged-in.png)

You can now configure your OpenVPN server.

## 4. OpenVPN Connect

### A. for Mac OS

Download and open the .dmg installer.

Follow the on-screen instructions to install.

The OpenVPN icon will appear near the system clock.

You can connect to your server through this menu.

### B. For Windows

Download and open the .MSI installer.

Continue at the prompt.

![](\assets\hosting\windows-prompt.png)

After installation, the OpenVPN icon should appear in the tray next to the clock on your Windows taskbar.

![](\assets\hosting\windows-taskbar-icons.png)

Right click on the icon. In the pop-up menu click `[Your_Server’s_IP]`

You can now select your OpenVPN server to connect.

## 5. Using your OpenVPN server

When you connect to your OpenVPN server, all traffic from your computer will be routed through the server.

Your computer will be assigned a new IP address.