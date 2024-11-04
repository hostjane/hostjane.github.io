---
layout: default
title: Managed VPS on EC2
description: VPS Hosting docs and help tutorials
nav_order: 4
has_children: true
permalink: /vps-hosting/
---

Managed VPS on Amazon EC2 ![](/assets/wave.svg)
{: .fs-9 .no_toc }

[Managed VPS Hosting Plans](https://cloud.hostjane.com/vps-hosting/){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [About Amazon EC2 Bare-Metal](https://aws.amazon.com/about-aws/whats-new/2023/10/new-amazon-ec2-bare-metal-instances/){: .btn .fs-5 .mb-4 .mb-md-0 }

# VPS Services Available
{: .no_toc }

- [x] Managed [cPanel / WHM VPS](/vps-hosting-tutorials/cpanel-whm/) on bare-metal EC2 instances
- [x] Managed [Plesk VPS](/vps-hosting-tutorials/plesk/) on bare-metal EC2 instances
- [x] Managed [DirectAdmin](/vps-hosting-tutorials/directadmin/) on bare-metal Amazon EC2 instances.
{: .fs-6 .fw-300 }

# Overview
{: .no_toc }

[Amazon Elastic Compute Cloud](https://aws.amazon.com/ec2/) (EC2) offers the most advanced server hardware available today, including VPS, or Virtual Private Servers. Think of VPS as isolated, virtual environments, being hosted on top of one big, physical Amazon bare-metal server. It's done through software called a *hypervisor*.
{: .fs-6 .fw-300 }

<iframe width="560" height="315" src="https://www.youtube.com/embed/q6WlzHLxNKI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

The hypervisor splits the computing resources of the underlying single physical machine—the server's memory or RAM, processing power or CPU, and the storage disk—into a pool of compartments or mini virtual machines, which are the VPS. Each VPS shares resources with the massive underlying server and gives dedicated-like performance to your website or app.
{: .fs-6 .fw-300 }

<span class="green">Watch this video to hear Tony explain VPS with helpful pictures.</span>
{: .fs-6 .fw-300 }

<iframe width="560" height="315" src="https://www.youtube.com/embed/GQwBzdYRS_c" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<span class="yellow">HostJane uses a [Type 1 Hypervisor](https://www.techtarget.com/searchitoperations/tip/Whats-the-difference-between-Type-1-vs-Type-2-hypervisor) to run VPS on powerful [Amazon Elastic Compute Cloud](https://aws.amazon.com/ec2/) (EC2) bare-metal instances, giving SMBs access to the same hardware used by multinational conglomerates, while keeping costs minimal.</span>
{: .fs-6 .fw-300 }

---

# Virtual Private Server FAQs
{: .no_toc }

## 5 Minute Read
{: .no_toc .text-delta }

1. TOC
{:toc}

## Why choose VPS over Shared hosting?

VPS on Amazon EC2 is a long-term investment in growth and sustainability. As described above, a Virtual Private Server (VPS) affords you a direct, protected share of a large physical bare-metal server. This means you won't be sharing computing resources like CPU, RAM, storage, and bandwidth, and will have root access to the server to install your own custom software and tailor applications for your own use with minimal restrictions.
{: .fs-6 .fw-300 }

<span class="green">Your website or apps needs won't be compromised by the processing and memory needs of "noisy neighbors" sharing the allocated resources of a server, insulating your site from common problems faced when hundreds of different businesses share the same resources.</span>
{: .fs-6 .fw-300 }

## Which AWS datacenter do you use?

<span class="blue">Currently HostJane is proud to manage VPS on Amazon EC2 for individuals and businesses in 14 global AWS datacenter locations including [N. Virginia region](https://www.aboutamazon.com/news/aws/aws-commitment-to-virginia).</span>
{: .fs-6 .fw-300 }

## Why pay HostJane if I can pay Amazon direct?

If you have the training and time to set up and run your own unmanaged linux or Windows server, and are happy to pay for and install your own SSL certificates, we recommend you do that. HostJane is aimed at busy startup and mid-level businesses, and owners, who want to outsource their IT service management and linux administration, with free SSL, to a qualified server team.
{: .fs-6 .fw-300 }

<span class="yellow">From Amazon server set up and hardening, to virtualization, server security, patching, updates, regular monitoring, event response, and technical support, we are here to help you make the most of AWS's incredible web offerings, 24/7, 365 days a year.</span>
{: .fs-6 .fw-300 }

HostJane strives to create a perfectly working server environment for each customer. Our goal is that you can spend maximum time on your sales, business marketing and non-IT operations, and minimal time on your website or app which will always be online and ready for your customers, on Amazon EC2, the world's most powerful server hardware.
{: .fs-6 .fw-300 }

## How long does server setup and provisioning take?

HostJane uses [Amazon EC2 API](https://docs.aws.amazon.com/AWSEC2/latest/APIReference/Welcome.html) to instantly provision your server. Amazon assigns an elastic IPv4 immediately, and server root access is available immediately. However, cPanel and Plesk application username and password are sent *by the server* after the installation finishes, which takes longer than standalone operation systems.
{: .fs-6 .fw-300 }

| VPS Software       | Time from payment |
|:-------------|:------------------|
| DirectAdmin           | After 40 mins you'll receive your DirectAdmin credentials |
| cPanel/WHM | 30-40 minutes installation time. The new server sends cPanel Admin username and password after install completes. |
| Plesk        | After 40 mins you'll receive the Plesk one-time link sent to your account email by the server |

<span class="red">Contact HostJane immediately if you have not received your cPanel admin username and password or Plesk one-time activation link after 1 hour from purchase.</span>
{: .fs-6 .fw-300 }

## What software can I use to manage my VPS?

HostJane offers managed [cPanel / WHM VPS](https://cloud.hostjane.com/vps/?appType=0&app=0) and [Plesk VPS](https://cloud.hostjane.com/vps/?appType=0&app=2) on bare-metal EC2 instances, provisioned with 14-Day trial licenses, and managed [DirectAdmin](https://cloud.hostjane.com/vps/?appType=0&app=1) on bare-metal EC2 instances.
{: .fs-6 .fw-300 }

<span class="yellow">After the 14-Day trial period, you will need to buy a license from cPanel or Plesk.</span>

[cPanel License Pricing](https://cpanel.net/pricing/){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [Plesk License pricing](hhttps://www.plesk.com/pricing/){: .btn .fs-5 .mb-4 .mb-md-0 }

## What content can I host on HostJane?

Ultimately, these are Amazon's servers. While we respect the privacy of our customers files, we do expect customers to comply with [HostJane AUP](https://www.hostjane.com/legal/use-policy/) and [HostJane Hosting TOS](https://www.hostjane.com/legal/hosting-terms), which will ensure you are aligned with AWS's expectations.

<span class="blue">As a rule of thumb, as long as whatever is on your website can be defined as “legal” in the United States, you won’t have any problems at HostJane.</span>

## Are backups included in server costs?

We offer 2 backup options, which are paid additional options in line with Amazon block storage pricing.

- [x] **Automated backups** which takes a complete snapshot of your entire Amazon VPS machine including all databases and files, every day at 2300 PST for 7 days consecutively, overwriting the first snapshot on Day 8. 
- [x] **Take My Own Snapshots**, which enables you to take and store up to 3 snapshots of your server per month.

##  Limits on Hosting Support

HostJane admins manage your Amazon EC2 server for reliability and uptime purposes, however our staff are not your web designers, advisors, or site developers.

### What can we help with?
{: .no_toc }

Open a support case for help with the following types of issue:

- [x] Any Amazon EC2 related issue
- [x] Server infrastructure issues
- [x] SSL issues related to your free, auto-renewing SSL certificate provided with the server
- [x] Server up-time issues
- [x] Moving your website to Amazon for a standard paid fee of $149.99
- [x] DNS issues at server level
- [x] Updates and patches
- [x] System critical functions
- [x] Server misconfigurations or usability problems

### What is beyond our scope
{: .no_toc }

- [x] Designing your website or app
- [x] Installing or configuring third-party software on your website or app
- [x] Fixing or controlling bugs in your website or app

<span class="purple">Please contact a freelancer on [HostJane marketplace](https://www.hostjane.com/marketplace) if you need help with bug fixes, developing or designing your website.</span>
