---
layout: default
title: VPS Hosting
description: VPS Hosting docs and help tutorials
nav_order: 6
has_children: true
permalink: /vps-hosting/
---

# Introducing HostJane VPS
{: .no_toc }

<span class="blue">Across 8 global AWS datacenters, HostJane VPS offers lightning-fast, managed VPS backed by the power and reliability of AWS.</span>

## In this section
{: .no_toc .text-delta }

1. TOC
{:toc}

# Core Features

| Feature |	Description |
|:-------------|:------------------|
| 24/7 human support |	HostJane's professional admins can assist you night and day. Our customer service team is passionate about giving accurate, support that resolves your issues first time. |
| 24-hour backups |	Your data is safe and securely backed up on a 24-hour cycle for a small fee. We can restore your server up to 5 earlier versions. |
| Free SSL	| HostJane can install a free Let's Encrypt SSL certificate that self-renews every 3 months. With root access or through cPanel, you can install any commercial SSL. |
| Managed server	| HostJane secures, monitors, and keeps your server stable. We deal with all software updates, stack issues, malware removal, and security patches. |
| Latest technology	| HostJane supports the latest versions of the best programming languages, including PHP, MySQL, Perl, and Python, to name a few. |
| Root access	| Maintain total control over your server’s configuration with root password access. [Contact us](https://www.hostjane.com/marketplace/support-root-access) for root access. |
| Dedicated IP	| There is an AWS IPv4 associated with your VPS. |

## Fully-managed hosting

All HostJane servers are AWS instances with an Amazon dedicated IP, protected by AWS Shield. HostJane will manage your VPS instance to ensure your web server is always online, kept up-to-date, any core updates or patches performed, and all technical problems concerning the server resolved.

## Zero Tolerance Spam policy

HostJane operates a zero tolerance on spam policy on all our plans.

## Bandwidth overages

1. You will receive an email asking you to upgrade to a new plan, or reduce usage.
2. If not practical and your server continues above the bandwidth threshold to prevent any bandwidth overage charges, the server will be stopped. 
3. There are no overage charges.

## cPanel License

We usually sell new servers with a Solo or trial cPanel license. Once the 15 day period has elapsed, we will upgrade the license. Customer takes no action.

## Content policy

- [x] While we respect the privacy of our customers files, we do expect customers to comply with [our AUP](https://www.hostjane.com/legal/use-policy/) and [hosting terms of service](https://www.hostjane.com/legal/hosting-terms).
- [x] As a rule of thumb, as long as whatever is on your website can be defined as “legal” in the United States, you won’t have any problems at this host.

## Daily backups

- [x] If selected during checkout, HostJane will perform daily backups of your AWS server including all files and databases.
- [x] We generally always have at least 5-7 past backups of the entire VPS servers in our system.
- [x] To request a restoration from a past backup, please contact us. There are no fees for this request.

## DDoS protection

Your server is at AWS and is shielded from most common forms of Distributed Denial of Service (DDoS) attack via AWS Cloud which has a free anti-DDoS system that analyzes, filters, and blocks malicious events.

**This includes protection against:**

- [x] User Datagram Protocol (UDP) packets: Where server ports are targeted by attackers.
- [x] Syn TCP and Ping attacks: Designed to overwhelm server resources forcing you offline.
- [x] Other amplification-based attacks like Network Time Protocol (NTP) and Domain Name Server (DNS) response traffic attacks

*Customers should be aware that no system however protected is DDoS proof. AWS VPS network will protect you against the most common volume-based and protocol floods.*

## Refunds

View HostJane's [refund policy](https://www.hostjane.com/legal/hosting-terms/) under Term 7.1 of our Hosting terms of service. Due to the nature of AWS server provisioning, we cannot provide prorated refunds.

## Cancellation

To cancel your subscription, please use the email you paid with to access the [Stripe billing portal](https://billing.stripe.com/p/login/3cs9AL9Aocs5dz2dQQ).

# What is a Virtual Private Server?

A [virtual private server](https://cloud.google.com/learn/what-is-a-virtual-private-server) is like a virtual compartment on a physical AWS server, guaranteeing you resources that simulate a dedicated environment.

![](/assets/hosting/how-web-hosting-works.svg)

Your website is made up of "files" called web pages. For people to access and read your site's files—doesn't matter if they're using a computer in your street or on the other side of the world—2 things need to happen:

1. Your files need to be stored on a server that can exchange information with other computers and servers anywhere. Your web server is like the hard drive on your own computer, but makes your files public.

2. The web server your files are stored on needs to have a unique, public address. We call this address your nameservers, and they are part of the Domain Name System (DNS), so other computers can find you.

When you host your website with HostJane, you are buying space and resources on a powerful AWS server for your files, and an assigned public address.

### Choose a VPS if:

1. You don't want your website disrupted by minute or large changes from thousands of other sites on a shared server
2. You are aiming to break into the Alexa Top 20,000 of most trafficked sites
3. Your site is scaling for medium to large traffic
4. You are hosting an application with resource intensive software scripts

### Pointing your domain

Please refer to our guide on [how to create an A record](https://help.hostjane.com/vps-hosting/point-your-domain/). Instructions are also sent on purchase.

Please contact your domain registrar's support if you need advanced DNS support.

### Windows dedicated servers

At present, HostJane only offers linux servers.

### No RAID-1 storage

HostJane doesn't use mirrored RAID.

Although RAID can protect against hardware failures that can takeout data striped storage (where data is written in blocks across 2 or more disks), if a virus corrupts one of your disks, those exact problems get replicated onto the "mirrored" disks and they get similarly destroyed leading to complete data loss.

Our 24-hr backups and any disk snapshots taken of your server get stored on AWS systems, making sure your data is always independently available for your users in the event of a server incident.

# Limits on Hosting Support

HostJane strives to provide 100% uptime and server reliability in keeping your website fast and always up.

However, our staff are not your individual web designers or site developers.

Please contact a freelancer on our marketplace if you need help with bug fixes, developing or designing your website.

#### What can we help with?

Open a support case for help with the following types of issue:

- [x] Server infrastructure issues
- [x] Server up-time
- [x] DNS issues at server level
- [x] Updates and patches
- [x] System critical functions
- [x] cPanel misconfigurations or usability problems

#### Web design, bug fixing & development support

[HostJane marketplace](https://www.hostjane.com/marketplace) connects you with freelance web, mobile, and software developers at fixed-prices, with a buyer money-back guarantee if work is unsatisfactory or late.

The marketplace is a great place to address issues such as:

- [x] Website design issues
- [x] Helping you learn how to code
- [x] Developing your website or application
- [x] DNS or domain problems at registrar level
- [x] Webmail/email issues where the server is working
- [x] Tutorials on using cPanel