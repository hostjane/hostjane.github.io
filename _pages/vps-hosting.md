---
layout: default
title: VPS Hosting
description: VPS Hosting docs and help tutorials
nav_order: 6
has_children: true
permalink: /vps-hosting/
---

# Introducing HostJane VPS

Across 17 global datacenters, HostJane VPS offers lightning-fast, managed SSD KVM VPS with the power and reliability of a dedicated server.

1. TOC
{:toc}

# Core Features

| Feature |	Description |
|:-------------|:------------------|
| 24/7 human support |	HostJane's professional admins can assist you night and day. Our customer service team is passionate about giving accurate, support that resolves your issues first time. |
| 24-hour backups |	Your data is safe and securely backed up on a 24-hour cycle for a small fee. We don't charge for back up storage. We can restore your server to 2 earlier versions. |
| Free SSL	| JaneVPS gives you a free SSL certificate that self-renews every 3 to 6 months. With root access or through cPanel or Plesk, you can install any commercial SSL. |
| Managed options	| Choose a self-managed linux server or managed environment with control panel. For managed options, JaneVPS secures, monitors, and keeps your server stable. We deal with all software updates, stack issues, malware removal, and security patches. |
| Latest technology	| JaneVPS supports the latest versions of the best programming languages, including PHP, MySQL, Perl, and Python, to name a few. |
| Scalable	| When your site’s space and bandwidth needs increasing, JaneVPS is nimble and flexible enough to instantly scale up with ease. Pay only for what you need at the time. |
| Root access	| Maintain total control over your server’s configuration with root password access.  JaneVPS has no restrictions including: unlimited domains, sub-domains, emails, MySQL databases, FTP accounts, metrics. |
| Extreme Speed	  | JaneVPS runs lightning-fast Intel® Skylake servers that use Solid-State-Drive storage which have no moving parts inside. |
| Dedicated IP	| The IPv4 associated with your JaneVPS is stable and mapped permanently to the server. You can add 1 additional IPv4 to each VPS you purchase. |
| Private eyes	| If what you’re building or running needs to be behind closed doors, JaneVPS’ firewall can give you 100% privacy. Only you and those white-listed devices will be able to see your server. Contact support to set up a firewall. |

## Fully-managed hosting

1. All HostJane servers are fully-managed for you by a team of experts. We back-up and secure your VPS for you.
2. If you want to be free of the technical responsibility required to keep a production linux server, up and stable throughout the year, HostJane VPS is for you.
3. We're often asked what does "fully managed” hosting mean in comparison to self-managed hosting? As an analogy, think of fully-managed like driving a car without needing to know how the carburetor works.
4. With HostJane, we are your website’s mechanics and pilots, letting you get on with your business.
5. Most importantly, “fully managed” means that we will help you resolve glitches, core updates, patches, and all technical problems you encounter.

## Email handling policy

1. JaneVPS allows the freedom to handle DNS records essential for mail delivery and spam protection either locally on the server, at your domain registrar, or with a third-party of your choice.
2. You can create unlimited email addresses. e.g. When JaneVPS runs cPanel/WHM app, the server is powerful enough to let you configure MX records, or POP3 and IMAP email locally on the server, or to let your domain registrar’s DNS handle that.
3. Mailing needs for our non-cPanel VPS instances, e.g. running Joomla, WordPress, or Drupal can also be configured locally on the server.
4. HostJane operates a zero tolerance on spam policy. 

## Bandwidth overages

1. You will receive an email informing you to upgrade your server and offering options.
2. If not practical and your server continues above the bandwidth threshold to prevent any bandwidth overage charges, the server will be stopped.

## Temporary SSL warning

1. Open a support case and tell us to install your free SSL certificate.
2. You’ll first need to point your domain to your server’s A-record which can take up to 72 hours to propagate (though is usually much faster).
3. DNS takes that long to propagate, which means updating Internet Service Provider (ISP) database nodes around the world. This is the case with any host, regardless of who they are. Unfortunately, while jane is super-fast, she can’t speed up the internet just for you.

## Linux distributions

With the exception of cPanel/WHM VPS which runs on CentOS, all HostJane VPS servers use the latest Ubuntu version.

## Special configurations

We can provide cPanel/WHM on Centos 6 if needed, and Webmin on CentOS 7 and CentOS 6 if you contact us to make a special order at the same prices.

## Content policy

- [x] We don’t police our customers files, so it’s up to you to ensure you are complying with our AUP.
- [x] As a rule of thumb, as long as whatever is on your website can be defined as “legal” in the United States, you won’t have any problems at this host.

## Automatic backups

- [x] HostJane can nightly backups of your entire server files and databases for a small fee.
- [x] We generally always have at least 2 past backups of the entire VPS servers in our system.
- [x] HostJane begins overwriting past backups, after 72 hours of storage.
- [x] To request a restoration from a past backup, please contact us. There is a $15 data restore admin fee.

*Note the restoration process can take up to 60 minutes and during that time your server may be unavailable.*

## Private builds

Do you need to build your website privately before going live?

There are 2 methods we recommend:

### A. Wait to change DNS

The first method is to wait to point your domain to the server and complete the site build first.

You can access your server by pointing your browser to its IP address.

{% highlight markdown %}
For example, by typing: HTTPS://[YOUR_SERVER_IP] in Firefox or Chrome.
{% endhighlight %}

- [x] Search engines won’t pick up your website content while it’s using an IP address.
- [x] It’s safe to ignore the temporary SSL browser warning during this time, which happens because it’s using a self-signed SSL certificate.
- [x] When you’re ready to go live, point your domain and we can install your free SSL certificate to remove the browser warning.

### B. Private eyes

The second method to run a private server is to request HostJane to set up a firewall on your server so only you (and the people you want to) can see your server.

## DDoS protection

During the most common forms of Distributed Denial of Service (DDoS) attack, JaneVPS has an anti-DDoS system that analyzes, filters, and blocks malicious events.

**This includes protection against:**

- [x] User Datagram Protocol (UDP) packets: Where server ports are targeted by attackers.
- [x] Syn TCP and Ping attacks: Designed to overwhelm server resources forcing you offline.
- [x] Other amplification-based attacks like Network Time Protocol (NTP) and Domain Name Server (DNS) response traffic attacks

*Customers should be aware that no system however protected is DDoS proof. HostJane VPS network will protect you against the most common volume-based and protocol floods.*


## Solid State Drives

HDDs contain lots of tiny, moving parts inside— like spinning plates, magnetic heads, and spindles—which can easily screw up causing data loss.

- [x] Unlike other hosts, HostJane only uses Solid State Drives (called SSDs) which make the read/write speed of your data and apps faster and more reliable.
- [x] SSDs are better because they have no moving parts inside to slow them down, giving our servers 3 major advantages:

1. **Read/write speed**: HostJane's SSDs compute faster which improves website loading times, makes apps faster, and increases productivity.
2. **Smarter**: Made from silicon memory chips, HostJane's SSDs have less power consumption than HDDs, which we pass on as cost savings to you.
3. **Tougher**: With no motorized spinning parts, HostJane's SSDs generate less heat making them less likely to burn out or fail, and longer lasting.
You can cancel your server at any time from your Hosting Portal account.

## Refunds

View HostJane's refund policy. Due to the nature of server provisioning, we cannot provide prorated refunds unless the server is materially damaged.

## Cancellation

### 1) Login to the Hosting Portal

Navigate to Dashboard

Find the server you wish to destroy in the Services list.

| Package | Label | Term  | Date Created | Date Renews | Options |
|:-------|:----------|:------|:----------|:------|:------|
| VPS 25GB SSD | Domain.com | 1 month @ $0.00 | Jan 1 | Feb 1 |*Manage* |

### 2) Select Manage under Options

Select *Cancel Options* at the bottom of the Information tab.

#### Manage VPS 25GB SSD - Domain.com

| Package | Status|
|:-------|:----------|
| VPS 25GB SSD | Active|
| **Label** | **Renew Date**|
| Domain.com | Feb 1 |
| **Creation Date** | **Next Invoice**|
| Jan 1 | Feb 1 |
| **Billing Cycle** | **Recurring Amount**|
| 1 Month | $0.00 |

#### Configurable Options

|:-------|:----------|
| **Additional IPv4 address** | Removed |
| **Backups** | Enabled |

#### Actions

|:-------|:----------|
| *Cancel Options* | Change Configurable Options |


### 3) Select Cancellation Type

1. You can choose to cancel immediately or at the end of the current monthly term.
2. You will need to confirm your Hosting Portal account password to proceed with termination.

#### Cancel Service

|:-------|:----------|
| Are you sure you want to cancel this service? |
| - [x] At End of Term (Jan 31) |
| - [] Immediately |
| - [] Do not cancel |

### Danger Zone

Cancellation is immediate and not reversible. All data is destroyed.

---

# Reseller VPS FAQs

## Managed, white-label VPS solution

JaneSells lets you resell high-quality, white-label VPS as servers in your own hosting operation. You independently manage your own clients.

**No one will see, not even in reverse IP lookups or advanced DNS tools, that you’re reselling HostJane.**

## How can I restore my clients' servers?

Open a ticket with our support team.

 - [x] HostJane makes nightly backups of your entire server files and databases for a small fee.
 - [x] We do not charge for backup storage.
 - [x] We always have at least 2 past backups of the entire VPS servers in our system.
 - [x] HostJane begins overwriting past backups, after 72 hours of storage.
 - [x] To request a restoration from a past backup on behalf of your customer, please contact us.
 - [x] Note there is a $15 data restore admin fee, that you should pass on to your customer.

*We recommend you also inform them that the restoration process can take up to 60 minutes and during that time your server may be unavailable.*

## Do you monitor my customers?

No. We expect you through our [Terms of Service](https://www.hostjane.com/legal/tos/) to ensure that whatever you or your clients are doing on the servers complies with US laws.

## Does JaneSells include DDOS protection?

Yes, to the same extent as regular HostJane VPS service provides.

---

# Why choose a VPS?

### What is shared hosting?

Your website is made up of "files" called web pages. For people to access and read your site's files—doesn't matter if they're using a computer in your street or on the other side of the world—2 things need to happen:

1. Your files need to be stored on a server that can exchange information with other computers and servers anywhere. Your web server is like the hard drive on your own computer, but makes your files public.
2. The web server your files are stored on needs to have a unique, public address. We call this address your nameservers, and they are part of the Domain Name System (DNS), so other computers can find you.

When you host your website, you are buying space on a server for their files, and an assigned public address.

![](/assets/hosting/how-web-hosting-works.svg)

#### The key difference

- With shared hosting, you are sharing server resources. With VPS, you have your own compartment.

- Though sub dollar pricing is attractive, shared hosts notoriously cram as many customers as possible onto a web server, severely restricting performance of your website.

#### Choose a VPS if:

1. You don't want your website disrupted by minute or large changes from the thousands of other sites on the same server as you;
2. You are aiming to break into the Alexa Top 20,000 of most trafficked sites;
3. Your site is scaling for medium to large traffic;
4. You are hosting an application with resource intensive software scripts

When we first started, HostJane provided free migrations to a shared hosting service, Plainspeed, which we terminated before cPanel moved to account-based pricing because we believe VPS is a better strategy for small website owners.

![](/assets/hosting/hostjane-free-migration.gif)

HostJane VPS are cheap, fast (because we separate all your files on the server in a "virtualization layer" to minimize disruption). and a workable alternative to having a dedicated server.

---

# Why upgrade to Dedicated?

1. Single-tenant SSD enterprise grade servers
2. Fully managed dedicated servers with up to 16 cores.
3. Built for resource-intensive sites.
4. Support massive, prime-time volume traffic.

| Features | HostJane Dedicated |
|:-------|:----------|
| 2 Dedicated IPs	| Your single-tenant, SSD dedicated server has 2 permanent, dedicated IPv4 addresses, with IPv6 capabilities. |
| Live human support	| Chat to your tech team 24×7, 365 days. We keep your server stable, backed up, patched, and clean of all malware. |
| Choose from 17 Datacenters	|  Designed for resource-intensive projects, HostJane Dedicated offers a truly global network of datacenters with the most powerful regional transit providers. |
| Free SSL certificates	| HostJane Dedicated comes equipped with an SSL certificate that self-renews every few months, or install your own. |
| Total privacy		| If what you’re building or running needs to be behind closed doors, our firewall can give you 100% privacy. Only you and those white-listed devices will be able to see your server. Contact support to set up a firewall. |
| DDoS Protection		|  Distributed Denial-of-Service Attacks (DDoS) are an increasing and ever-present threat where criminals flood their victim (the server) with so many global requests, it’s resources are overloaded. Worse case scenario, the server can become unusable and all data is destroyed. DDoS attacks can wreak financial havoc for victims, especially online businesses where every minute of downtime is lost money. In a DDoS attack, HostJane Dedicated will be your site’s guardian angel. She blocks the crossfire in real-time, and helps reduce the risk and damage caused to your server. Included free in all Dedicated servers. |
| Automatic backups for less	| We treat your server as mission-critical. We ensure your sensitive, crucial data is backed up on multiple servers every day. You can also initiate snapshots of your server’s volume in any of our global datacenters, stored free-of-charge. With HostJane Dedicated you have extreme speed, verifiable bandwidth, and the backup capabilities of a major player. |
| Email Handling | 	Configure email DNS records locally (at no added cost) on the server with HostJane Dedicated, or devolve your email handling to your registrar or use another service. It’s entirely up to you. For example, if you wished to use Gmail for business with Google’s G-Suite apps, you could add the Google MX records locally on your server or at your registrar, and either method should work. Importantly, you can set-up unlimited email accounts with no restrictions. |

### Dedicated hosting
HostJane's dedicated servers offer premium, state-of-the-art hardware backed by our 100% SLA.

**You are the single occupant on the server no neighbors, and you customize every aspect of the server and all its resources to your needs.**

Our dedicated environment generally makes your website more secure, and gives more consistent server performance over time.

Think of hosting your website on a server like buying in an apartment building:

 - [x] Shared hosting buys you a condo, where you'll have to share amenities with other tenants on your floor and other floors in the building;
 - [x] VPS hosting buys you an entire floor in the building, giving you more room and more resources;
 - [x] Dedicated hosting gives you the entire building complex – all cores, memory and disk storage – all devoted to your website's needs.

### Domain pointing

Please refer to our guide on how to create an A record. Instructions are also sent on purchase.

Please contact your domain registrar's support if you need advanced DNS support.

### Windows dedicated servers

At present, HostJane only offers linux servers.

### Upgrading to HostJane Dedicated

Yes, you can at any time and one of the conveniences of HostJane is that any VPS backups and snapshots taken are immediately moved to the new server.

Unlike many hosts, we don't nickel and dime our customers by charging people to make backups of dedicated storage by the gigabyte when they are already making such a big investment in the server.

### No RAID-1 storage

HostJane doesn't use mirrored RAID.

1. Although RAID can protect against hardware failures that can takeout data striped storage (where data is written in blocks across 2 or more disks), if a virus corrupts one of your disks, those exact problems get replicated onto the "mirrored" disks and they get similarly destroyed leading to complete data loss.
2. HostJane Dedicated uses a proprietary storage structure that has multiple layers of in-built data protection.
HostJane Dedicated provides greater "redundancy" than RAID-using hosts i.e. backups across the network that add a greater degree of security for your data.
3. Both our 24-hr backups and any disk snapshots you take of your own server also gets stored on these redundant systems, making sure your data is always independently available for your users in the event of a server incident.

### Automatic backups

- HostJane can make nightly backups of your entire dedicated server files and databases for a much smaller fee than most dedicated hosts. We also don't charge for backup storage. We generally always have at least 2 past backups of your site in our system.
- We begin overwriting past backups, after 72 hours of storage. To request a restoration from a past backup, please contact us. There is a $15 data restore admin fee.
- Note the restoration process can take up to 60 minutes and during that time your server may be unavailable. 

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

# About Console

Managing your servers has never been easier with the new HostJane Console, a secure client-side billing & server provisioning app. 

![](/assets/hosting/console.jpeg)

Console has 2-factor authentication & industry-standard encryption: Bcrypt HMAC SHA-256 hashes for passwords. AES-256 & RSA for data. 

Easy to use over mobile, tablet & desktop, Console allows you to assign roles to different team members restricting specific privileges in your account on a per user basis. Update or change payment information, get up-to-date systems information on your servers. Start, restart, stop & cancel servers in a few easy clicks. 

![](/assets/hosting/hosting.png)

Console is linked to the HostJane server wizards and provides instant access to root passwords, server information, usage data, operating systems and more. Track CPU usage, disk operations & easily request to scale your server to suit your needs.

Whether you're a server administrator running a linux compute or self-employed beginner using a VPS cPanel or preinstalled WordPress VPS, HostJane Console offers an accessible suite of system, billing & invoice tools to remotely manage your server from anywhere.