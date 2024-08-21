---
layout: default
title: Point your domain to your hosting
description: How to point your domain A-record to your VPS or Amazon EC2 Instance
nav_order: 1
permalink: /point-your-domain/
---

# Point your domain to hosting ![](/assets/wave.svg)
{: .fs-9 .no_toc }

There are 3 easy steps to see your website, on your new Amazon EC2 server, in any web browser. *First*, login to your domain registrar. *Second*, map an A-Record at your registrar, to your new Amazon server's IP address. *Third*, check you've done it right.
{: .fs-6 .fw-300 }

## Quick Start Summary
{: .no_toc .text-delta }

1. TOC
{:toc}

## First, find your domain registrar

Your registrar is the place you either **bought** or **transferred** your domain. 

<span class="green">Your domain's records are managed at the registrar.</span>

The first step is to logon to your registrar and navigate to your domain's control panel. 

|   ![](/assets/one.svg)           | The first step is to logon to your registrar and navigate to your domain's control panel. Links to the largest domain registrars are below. |

<span class="yellow">Links to the largest domain registrars are below.</span>

| Registrar	| Instructions |
|:-------------|:------------------|
| 1&1 IONOS	| [Open Link](https://www.ionos.com/help/domains/dns-settings/) |
| Amazon Route 53 | [Open Link](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/resource-record-sets-creating.html) |
| Alibaba Cloud | [Open Link](https://www.alibabacloud.com/help/en/dns/add-an-a-record-to-a-website-domain) |
| Ascio | [Open Link](https://aws.ascio.info/AscioDns/nodejs/updaterecord) |
| Cloudflare | [Open Link](https://developers.cloudflare.com/dns/manage-dns-records/how-to/create-dns-records/) |
| Dynadot	| [Open Link](https://www.dynadot.com/community/help/question/create-A-record) |
| eNom |	[Open Link](https://www.enom.com/kb/kb/kb_0002_change-host-records.htm) |
| Google Domains |	[Open Link](https://support.google.com/domains/answer/9211383) |
| GoDaddy |	[Open Link](https://godaddy.com/help/add-an-a-record-19238) |
| Network Solutions |	[Open Link](http://www.networksolutions.com/support/a-records-ip-addresses-2/) |
| Gandi	| [Open Link](https://wiki.gandi.net/en/dns/zone/edit) |
| Hover |	[Open Link](https://help.hover.com/hc/en-us/articles/217282457-How-to-Edit-DNS-records-A-AAAA-CNAME-MX-TXT-SRV-) |
| NameCheap |	[Open Link](https://www.namecheap.com/support/knowledgebase/article.aspx/319/2237/how-can-i-set-up-an-a-address-record-for-my-domain/) |
| Name.com |	[Open Link](https://www.name.com/support/articles/205188538-Pointing-your-domain-to-hosting-with-A-records) |
| OVHcloud |	[Open Link](https://help.ovhcloud.com/csm/en-au-dns-edit-dns-zone?id=kb_article_view&sysparm_article=KB0051673) |
| Public Domain Registry |	[Open Link](https://pdrinc.myorderbox.com/kb/servlet/KBServlet/faq471.html) |
| Tucows Domains |	[Open Link](https://tucowsdomains.com/help/domain-management/change-my-dns-nameservers/) |

## Second, create an A-Record

|   ![](/assets/two.svg)           | The second step is to navigate to the DNS manager or DNS zone in your registrar, and either create a new A Record with your Server IP address or update the existing A record. |

## What is an A Record?
{: .no_toc }

<span class="yellow">Address (A) records, written for short as "A-records", are part of the DNS or [Domain Name System](https://www.cloudflare.com/en-gb/learning/dns/what-is-dns/), that point domains to IP addresses or servers.</span>

When a user wants to visit your website, their web browser (like Google Chrome) will ask your domain’s nameservers for the A-record.

<span class="red">NB: A website is made from its files and database hosted on a server.</span>
![](/assets/hosting/a-record-ipv4.svg)

The A-record at your nameserver connects to the IP address of your server.

<span class="green">Every server connected to the internet has an IP or *Internet Protocol* address.<span>

The IP address is the unique identifer of your server, connected to the internet, where your website's files and database is stored.

<span class="orange">Tony explains this perfectly.<span>

<iframe width="560" height="315" src="https://www.youtube.com/embed/QcNBLSSn8Vg
" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

So every time you look up a website in a web browser like Google Chrome, A-records are how your browser gets the directions of which IP address or server to connect to. As Tony said, this will work for any domain regardless of who you are registered with.

## Here's an example to help you
{: .no_toc }

Mary bought an Amazon EC2 server [running WordPress](https://cloud.hostjane.com/wordpress/), managed by HostJane. Her domain registrar is Amazon Route 53. 

<span class="blue">2-3 minutes after purchase, Amazon assigns Mary's new EC2 server an IPv4 address of: 123.456.789.1</span>

Mary's domain name is **example.com**

![](/assets/hosting/route53.png)

For Mary to see her server in her web browser, she logs on to her domain registrar, and navigates to the DNS manager or zone in the registrar's panel.

<span class="purple">Mary updates example.com's A-records as follows:</span>

| Host | 	Type | 	Data |
|:----------|:------------|:--------|
| @	 | A |	123.456.789.1 |
| www	| A	 | 123.456.789.1 |

<span class="blue">This set up will ensure the following:</span>

**example.com** will map to **123.456.789.1**

**www.example.com** will also point to **123.456.789.1**

<span class="purple">Route 53 only allows 1 entry, but if your registrar allows more than 1, use Mary's example.</span>

## What is my hostname?
{: .no_toc }

Your hostname is simply the label, in human words, for your Amazon server. It's usually your [fully qualified domain name](https://kb.iu.edu/d/aiuv) (FQDN), e.g. www.example.com.

<span class="yellow">If you get a chance, create an A record for both the non-www and www version of your domain name. That way, both www.example.com and example.com will point (or resolve) to your Amazon server.</span>

This will prevent your website experiencing any issues with duplicate content or canonical problems that can affect website ranking.

### Tip - tell Google how your domain should be known
{: .no_toc }

It's a good idea to [add a "canonical tag" to your domain](https://moz.com/learn/seo/canonicalization) to tell Google if you want the www or non-www version of your site (example.com or www.example.com) to show to visitors when they visit your domain.

<span class="green">Use [Google Search Console](https://search.google.com/search-console/about) to help you do this.</span>

## Third, check your domain's DNS has propagated

|   ![](/assets/three.svg)           | The last step is to check at help site, [What's My DNS](https://www.whatsmydns.net/), that your A Record is correctly pointing to your new Server's IP address. If your plan includes free SSL, also check [SSLShopper](https://www.sslshopper.com/ssl-checker.html) that SSL is properly configured on your domain. |

## What is DNS?
{: .no_toc }

<span class="red">Your web browser read A-Records in the DNS or **D**omain **N**ame **S**ystem, which Cloudflare describes as the [phonebook of the internet](https://www.cloudflare.com/en-gb/learning/dns/what-is-dns/).</span>

A-Records point to IP addresses of servers. This is how web browsers can then connect across the internet to the server at Amazon where your website's files and databases will be stored.

## DNS Requests
{: .no_toc }

Geeks call IP addresses, “IP v4 addresses”, because they are mostly written as 4 sets of numbers separated by dots, i.e. 111 . 222 . 333 . 444

<span class="blue">Your IP address, and A-Record, are totally unique to your HostJane server and help people find you on the internet.</span>

Each HostJane server includes a unique Amazon IP address.

<span class="yellow">So that people don’t have to remember your website as a string of numbers, like 111.222.333.444, your domain's nameservers change those numbers, and computer talk, into simple human words.</span>

This way people can type www.yourwebsite.com into browsers (like Google Chrome, Mozilla Firefox and Apple Safari) to find the server holding your website’s files & databases online.

## Check domain is propagated
{: .no_toc }

We recommend using WhatsMyDNS.net to check on the progress of your A-record's propagation status.

<span class="green">Go to [What's My DNS](https://www.whatsmydns.net/)</span>

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
{: .no_toc }

These days, DNS propagation is usually super quick and propagated within 1-2 minutes. But technically it can take a lot longer for DNS to propagate. We recommend to contact your domain registrar's support if your domain's map at [What's My DNS](https://www.whatsmydns.net/) is not turning green after an hour.