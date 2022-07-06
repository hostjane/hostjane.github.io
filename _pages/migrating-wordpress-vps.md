---
layout: default
title: Moving to WordPress VPS
parent: VPS Hosting
description: How to migrate your WordPress site to HostJane VPS
nav_order: 13
permalink: /vps-hosting/migrating-wordpress-vps/
---

# Moving to WordPress VPS

<span class="green">HostJane recommends All-in-One WP Migration by ServMask, Inc. to migrate WordPress sites to HostJane. With over 1 million+ uses the plugin is the easiest way to move a WordPress site.</span>

1. TOC
{:toc}

## 1. Purchase a WordPress VPS

Use HostJane's Server Wizard to find the server size that's right for you. HostJane WordPress VPS runs directly on an Ubuntu linux distribution, without any third-party CMS.

Select Content Management Systems > WordPress

![](/assets/hosting/server-wizard.png)

You can run a WordPress VPS in up to 17 datacenter locations, we recommend choosing a location that nearest to your customers. 

## 2. Set up your WordPress VPS

Before you migrate your old WordPress site, setup your new WordPress VPS.

The new WordPress installation should be reachable in the browser at an IP address, for example: 123.456.789.1

## 3. Back up your old site

All-in-One WP Migration is easy to use, but care should be used with import/export options as it can affect your WordPress database.

It's best to back up your existing WordPress site at the start.

 <iframe width="560" height="315" src="https://www.youtube.com/embed/BpWxCeUWBOk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## 4. Export your old WordPress website

Login to your old WordPress host by going to /wp-admin/ or /wp-login.php/ at your existing site.

![](/assets/hosting/old-site.png)

Navigate to Plugins > Add Plugin

Type in All-in-One WP Migration until the ServMask plugin appears.

![](/assets/hosting/all-in-one-wp-migration.png)

Press Install > Activate

In the left-hand WordPress dashboard, you should see the All-in-One WP Migration tool appear.

![](/assets/hosting/all-in-one-wp-migration-export.png)

Go to All-in-One WP Migration > Export

![](/assets/hosting/all-in-one-wp-migration-export-file.png)

Choose File which will export your entire WordPress site as a .wpress file.

Unless you’re an experienced WP user, we don’t recommend adding any settings or changing any of the default Advanced Settings which may impact on the MySQL database you import to your new WordPress server.

You’ll see a few system messages, followed by the download button.

![](/assets/hosting/checking-extensions-compatibility.png)

The larger your website is, the more time it may take to archive the database.

![](/assets/hosting/done-archiving-database.png)

Eventually you’ll see a flashing green Download LocalHost button.

![](/assets/hosting/download-localhost.png)

Click Download to export your WordPress site as a .wpress file to your local computer.

## 5. Import your old WordPress site

We assume you have already set up your WordPress VPS so the new WordPress site is reachable in the browser.

In a new browser window, login to your new WordPress server’s /wp-admin/ dashboard area.

Install All-in-One WP Migration by navigating to Plugins > Add Plugin in your new WordPress site.

Find the plugin: All-in-One WP Migration

![](/assets/hosting/all-in-one-wp-migration.png)

Again, press Install > Activate

In the left-hand WordPress dashboard, you should see the All-in-One WP Migration tool appear.

As you want to import your old site to your new website, choose Import in the plugin’s dashboard menu.

![](/assets/hosting/all-in-one-wp-migration-import.png)

The All-in-One WP Migration import screen will appear.

![](/assets/hosting/all-in-one-wp-migration-import-file.png)

Select File from the Import dropdown.

Find the localhost.wpress file that you exported from your old host to your computer, and upload it at the prompt.

![](/assets/hosting/all-in-one-wp-migration-import-file-in-progress.png)

This can take time depending on your ISP’s speed and how big your old website is.

<span class="blue">Be prepared to wait up to 1 hour or more for the upload to finish.</span>

Do not close your browser while the file upload is in progress.

Upon completion you will get a warning message advising that you are about to overwrite ALL file and database data on your new WordPress VPS.

You are replacing your WordPress VPS's files with a perfect copy of your old website.

![](/assets/hosting/all-in-one-wp-migration-import-file-warning.png)

### Click Proceed to continue the transfer process.

Be warned this overwriting is not a reversible process.

If you have already started building your new website on your WordPress VPS and don’t wish to overwrite that data, you should use the backup feature in All-in-One migration to take a copy before you import your old site's wpress file.

![](/assets/hosting/all-in-one-wp-migration-import-success.png)

### Click Permalink Settings

Once the import has finished, you will be logged out of the new site.

Log back into your new WordPress server using your old site’s /wp-admin/ username and password credentials.

<span class="purple">This happens because when you import the data from your old site with the .wpress file, it overwrites your WordPress website’s MySQL database where usernames and password credentials are stored.</span>

We recommend updating the username and password to your new site, use a strong password generator to create a password longer than 16 characters that even hackers can’t manipulate.

## 6. Change your password

Don't use an easy password

Use a strong password generator to choose a secure, random password for your site.

## 7. Update Permalink Structure TWICE

Finally, in Permalink Settings, click Save Changes once.

Then wait until the Permalink structure has updated and save it again.

![](/assets/hosting/permalink-settings-updated.png)

Your new WordPress site should have been successfully imported!

Click Visit Site in the top left dropdown to visit your new Website.

If everything has gone well, you should see your old WordPress site on your new WordPress VPS with HostJane. Congratulations!

### Take a Snapshot for Extra Precautions

Keep in mind that if you want to backup your WordPress VPS for server to protect your data.

Login to the Hosting Portal and go to Snapshots in your WordPress server’s dashboard.

Take a backup copy of the entire server before you import the .wpress file, so you can restore by contacting us (admin fee applies).

| Package | Status|
|:-------|:----------|
| WordPress | Active|
| **Label** | **Renew Date**|
| Domain.com | Feb 1 |
| **Creation Date** | **Next Invoice**|
| Jan 1 | Feb 1 |
| **Billing Cycle** | **Recurring Amount**|
| 1 Month | $0.00 |

If you’re comfortable using a command line program like [WP-CLI](https://wp-cli.org/), ServMask’s All-in-One WP migration plugin [can be handled](https://help.servmask.com/knowledgebase/cli-integration/) from that interface.