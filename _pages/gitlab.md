---
layout: default
title: 1-Click GitLab
parent: Cloud Computes
description: How to setup a GitLab server
nav_order: 9
permalink: /cloud-compute/gitlab/
---

# 1-Click GitLab
{: .no_toc }

<span class="green">Tutorial for running latest GitLab version on HostJane.</span>

- HostJane’s cloud servers runs the GitLab Community Edition (CE) on Ubuntu. 
- Note that GitLab requires a cloud compute running at the minimum 2 CPU.

## In this section
{: .no_toc .text-delta }

1. TOC
{:toc}

## 1. Get server IP and root password

After successful payment is approved, your server will be set up within 2 minutes.

### A. Login to the Hosting Portal

Bookmark login: [https://console.hostjane.com/client/login](https://console.hostjane.com/client/login)

In your Dashboard under Services, find your GitLab server.

| Package | Label | Term  | Date Created | Date Renews | Options |
|:-------|:----------|:------|:----------|:------|:------|
| GitLab | host.domain.com | 1 month @ $0.00 | Jan 1 | Feb 1 |*Manage* |

We offer 24×7×365 support

If you cannot see your Debian service, open a support case.

### B. Click the Manage option

This is the button in the last column under Services.

Here is the next screen that will display: 

| Package | Status|
|:-------|:----------|
| GitLab | Active|
| **Label** | **Renew Date**|
| host.domain.com | Feb 1 |
| **Creation Date** | **Next Invoice**|
| Jan 1 | Feb 1 |
| **Billing Cycle** | **Recurring Amount**|
| 1 Month | $0.00 |

### C. Click *Statistics* in the side menu

| GitLab Server Details |
| Access your GitLab application by visiting this URL: |
| https://123.456.789.1 |
| User: root |
| Pass: demo123 |

In this example, the server link is: https://123.456.789.1

In this example case the IP is: 123.456.789.1

```
Your Server Link
https://[Your_Server’s_IP]/
```

For security, HostJane does not send this to you by email.

You must login to your hosting account to review these credentials.

## 2. Ignore the browser warning

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

## 3. Access the Gitlab installer

After passing the security dialog, you will see your server’s GitLab signin.

![](/assets/hosting/gitlab-community-edition-signin.png)

Copy and paste the root username and password as provided in Statistics to login to your GitLab portal:

![](/assets/hosting/gitlab-community-edition-loggedin.png)

## 4. Update your domain URL to GitLab configuration

It’s not enough to simply point your domain to your GitLab server, you need to ensure that clone URLs are not generated that could impede your workflow.

Login to your server with PuTTY on Windows or an OpenSSH client in linux and MacOS devices:

```
ssh -l root [Your_Server's_IP]
```

Once logged in as the root user, use the nano command-line text editor to edit the following file:

```
nano /etc/gitlab/gitlab.rb
```

![](/assets/hosting/gitlab-clone-urls.png)

Move the cursor to change the external_url from:

```
external_url https://[Your_Server's_IP]
```

Change to your domain:

```
external_url https://YourDomain.com
```

Press `ctrl + O` then Enter to write the changes to SSH daemon

Now close the file with `ctrl + x`

Reconfigure the GitLab server by typing:

```
gitlab-ctl reconfigure
```

You have successfully installed your Gitlab server!

All repositories created and managed through the GUI can be found located at:

```
/var/opt/gitlab/git-data/repositories
```