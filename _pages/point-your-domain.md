---
layout: default
title: Point Your Domain
parent: VPS Hosting
description: How to create a-records to point a domain
nav_order: 1
permalink: /vps-hosting/point-your-domain/
---

# How to Point Your Domain to Your Server

This article will explain how A-records work, then show you how you can create an A-record at the registrar where you purchased your domain.

1. TOC
{:toc}

## What are A-Records?

<span class="green">Address (A) records, written for short as "A-records", are part of the DNS or Domain Name System, that point domains to IP addresses.</span>

When a user wants to visit your website, their browser will ask your domain’s nameservers for the A-record.

![](/assets/hosting/a-record-ipv4.svg)

The A-record at your nameserver connects to the IP address of your server.

Every server connected to the internet has an IP address.
IP addresses are a fancy way of saying the label (or as geeks will tell you, Internet Protocol) of the server where a website's files and database is stored.

So every time you look up a website in a web browser like Google Chrome, A-records are how your browser gets the directions of which IP address or server to connect to.

## DNS Requests

Once your visitor's computer has got back this information off the nameserver, their web browser can then connect across the internet to the server at HostJane where your website's files and databases are located.

#### That's called a DNS Request.

Geeks call IP addresses, “IP v4 addresses”, because they are mostly written as 4 sets of numbers separated by dots, i.e. 111 . 222 . 333 . 444

<span class="blue">Your IP address, and A-Record, are totally unique to your HostJane server and help people find you on the internet.</span>

Each HostJane VPS server includes ONE unique (1) dedicated IPv4 address.

So that people don’t have to remember your website as a string of numbers, like 111.222.333.444, your domain's nameservers change those numbers & computer talk into simple human words.
This way people can type www.yourwebsite.com into browsers (like Google Chrome, Mozilla Firefox and Apple Safari) to find the server holding your website’s files & databases online.

### Create an A-record

In our example, your server has the IPv4 address of: 123.456.789.1 

Your domain is example.com.

Go to your domain registrar, navigate to the DNS manager or zone, and update the A-records as follows:

| Host | 	Type | 	Data |
|:----------|:------------|:--------|
| @	 | A |	123.456.789.1 |
| www	| A	 | 123.456.789.1 |

You can find instructions from popular registrars below.

#### Preventing duplication issues

By following our example above, you create an A record for both the non-www and www version of your domain.

Both www.example.com and example.com will point (or resolve) to the server.
We suggest this to prevent your website problems experiencing any issues with duplicate content and or canonical problems that can affect website ranking.

#### An example setup

example.com resolves to 123.456.789.1

www.example.com resolves to 123.456.789.1

It's a good idea to add code to your website to tell Google if you want the www or non-www version of your site (example.com or www.example.com) to show to visitors when they visit your domain.

We recommend using Google Search Console to help you do this.
This article from Moz can help you understand the issue so your website is consistent for search engines from the outset.

Contact your registrar if you need help with adding or changing an A-Record.

### Find your registrar

Below are links to instructions from the largest domain registrars on how to create your domain’s A-Record.

| Registrar	| Instructions |
|:-------------|:------------------|
| GoDaddy |	[Open Link](https://godaddy.com/help/add-an-a-record-19238) |
| Network Solutions |	[Open Link](http://www.networksolutions.com/support/a-records-ip-addresses-2/) |
| eNom |	[Open Link](https://www.enom.com/kb/kb/kb_0002_change-host-records.htm) |
| 1&1 IONOS	| [Open Link](https://www.ionos.com/help/domains/dns-settings/) |
| Google Domains |	[Open Link](https://support.google.com/domains/answer/9211383) |
| Dynadot	| [Open Link](https://www.dynadot.com/community/help/question/create-A-record) |
| Gandi	| [Open Link](https://wiki.gandi.net/en/dns/zone/edit) |
| Hover |	[Open Link](https://help.hover.com/hc/en-us/articles/217282457-How-to-Edit-DNS-records-A-AAAA-CNAME-MX-TXT-SRV-) |
| Name.com |	[Open Link](https://www.name.com/support/articles/205188538-Pointing-your-domain-to-hosting-with-A-records) |
| Public Domain Registry |	[Open Link](https://pdrinc.myorderbox.com/kb/servlet/KBServlet/faq471.html) |
| NameCheap |	[Open Link](https://www.namecheap.com/support/knowledgebase/article.aspx/319/2237/how-can-i-set-up-an-a-address-record-for-my-domain/) |

### Check domain is propagated

We recommend using WhatsMyDNS.net to check on the progress of your A-record's propagation status.

Go to WhatsMyDNS.net

Enter your domain in the main field, select A in the dropdown, and hit Search.

![](/assets/hosting/whatsmydns.png)


If your domain is successfully propagated, the map will show all green ticks.

![](/assets/hosting/propagation-successful.png)


When successful, each ISP country will show your A-record with a green tick.

![](/assets/hosting/fully-propagated.png)


Unfortunately we have to wait for ISP nodes around the world to update.

This can take up to 72 hours. During this time, the ISP nodes will show red crosses.

![](/assets/hosting/not-propagated.png)

The map will show red crosses during this transition time.

![](/assets/hosting/not-propagated-map.png)

While propagation is still pending, or has failed, there maybe a mixed-picture of red crosses and green ticks.

### Troubleshooting A-records

Remember it can take up to 72 hours for DNS to propagate. Contact your domain registrar's support if the map is not turning green after 72 hours.