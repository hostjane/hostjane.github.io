---
layout: default
title: Managed Cloud on EC2
description: Cloud hosting docs and help tutorials
nav_order: 3
has_children: true
permalink: /cloud-hosting/
---

Managed Cloud on Amazon EC2 ![](/assets/wave.svg)
{: .fs-9 .no_toc }

Improve your web offerings by moving your digital agency, ecommerce store, or online business to scalable Amazon EC2 virtual machines. Managed by HostJane's admin team, we can onboard every project, test server, website or app, to Amazon Web Services (AWS) at a low cost per month.
{: .fs-6 .fw-300 }

<iframe width="560" height="315" src="https://www.youtube.com/embed/q6WlzHLxNKI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

[Managed AWS EC2 Plans](https://cloud.hostjane.com/vps/?appType=0&app=0){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [Unmanaged Amazon EC2 pricing](https://aws.amazon.com/ec2/pricing/on-demand/){: .btn .fs-5 .mb-4 .mb-md-0 }

- [x] Managed [Laravel](/cloud-hosting/laravel/) on EC2 servers
- [x] Managed [LAMP](/cloud-hosting/lamp-php/) with PHP-FPM packaged on EC2 servers
- [x] Managed [Jupyter Notebook](/cloud-hosting/jupyter-notebook/) on EC2 servers
- [x] Managed [Django](/cloud-hosting/django/) on EC2 servers
- [x] Managed [Nginx](/cloud-hosting/nginx/) on EC2 servers
- [x] Managed [Windows Server](/cloud-hosting/windows-hosting/) on EC2 servers
{: .fs-6 .fw-300 }

---

# About the program
{: .no_toc }

<span class="blue">Currently HostJane is proud to manage VPS on Amazon EC2 for individuals and businesses in AWS's [Virginia region](https://www.aboutamazon.com/news/aws/aws-commitment-to-virginia). </span>

## In this section
{: .no_toc .text-delta }

1. TOC
{:toc}

# Why move to Amazon EC2?

Most people use [Amazon Web Services](https://aws.amazon.com/) or *AWS* without even knowing it, just by browsing the internet. So much of the internet relies on Amazon's giant infrastructure, including this one, you'll likely browse websites or apps running on Amazon virtual machines, each time you navigate from Google to a search result on your phone, tablet or desktop web browser.
{: .fs-6 .fw-300 }

Amazon is in fact so massive, unless you're NASA, you couldn't possibly outgrow Amazon's [Elastic Cloud Compute](https://aws.amazon.com/ec2/) or *EC2*. As demand for your service or website increases, Amazon's unlimited resources to scale, used by the world's largest enterprises, can support your business goals.
{: .fs-6 .fw-300 }

<iframe width="560" height="315" src="https://www.youtube.com/embed/iHX-jtKIVNA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<span class="green">Key benefits of using Amazon EC2 managed by HostJane</span>
{: .fs-6 .fw-300 }

- [x] Ability to scale - you can take over managing your HostJane-managed EC2 instance at any time, move to a bigger server with On-Demand, Reserved Instance, or Spot Instance pricing, add load balancers, add a CDN like Amazon CloudFront, all while staying within the security of Amazon's platform. 
- [x] Fastest data processing than any other web host can offer
- [x] Latest, most advanced hardware - compared to AWS everyone else is playing catch up
- [x] Global storage capacity
- [x] Improved website and server speed
- [x] Near 100% uptime reliability 
{: .fs-6 .fw-300 }

You can lift the entire user experience for your small or medium sized business by moving off whatever you are using to AWS's Elastic Compute Cloud, managed by HostJane, in Amazon's public cloud.
 {: .fs-6 .fw-300 }

# What is virtualization?

The [best definition belongs to Red Hat](https://www.redhat.com/en/topics/virtualization/what-is-virtualization), but, in a nutshell, *Virtualization* is technology that uses software called a *hypervisor* to split up the hardware of a single physical server. This means splitting up the underlying server's processors, storage, and memory, to create a pool of multiple operating systems and applications running on top of the server. 
 {: .fs-6 .fw-300 }

<span class="orange">Amazon calls these mini servers, virtual machines or VMs, which is the basic principle behind Amazon Elastic Compute Cloud.</span>
 {: .fs-6 .fw-300 }

![](/assets/virtualization.png)

*Image copyright courtesy of Red Hat, Inc.*

There are [5 essential features](https://nvlpubs.nist.gov/nistpubs/legacy/sp/nistspecialpublication800-145.pdf) of AWS's cloud computing.
 {: .fs-6 .fw-300 }

First, its global network, second the way it provides pooled resources and virtual machines for a tailored workload. Third, the way it gives its users a self-service interface to control, fourth, the way it can rapidly scale or *provision* those virtual machines, and finally, the way it automatically controls and allocates resources depending on use.
 {: .fs-6 .fw-300 }

# What's the difference between a Virtual Private Server (VPS) and cloud hosting?

While both use a hypervisor to in some way manage the resources of an underlying physical server (like CPU, RAM, Storage), VPS is limited to one server, while cloud computing technology spreads resources over a network of servers, making it much more stable and reliable, minimizing any [single point of failure](https://docs.aws.amazon.com/whitepapers/latest/real-time-communication-on-aws/high-availability-and-scalability-on-aws.html) if any part of the system fails.
 {: .fs-6 .fw-300 }

For example, the Amazon EC2 virtual machines that HostJane manages rely on Amazon's [elastic IP addresses](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/elastic-ip-addresses-eip.html), and [Elastic Block Storage](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/storage_ebs.html) (EBS), both of which can be attached and detached to and from different EC2 virtual machines in Amazon's public cloud to change IP or move stored data around, depending on needs.
 {: .fs-6 .fw-300 }

# What's the difference between a private and public cloud?

A *public cloud*, like Amazon EC2, is a pool of virtual machines run on datacenters owned by AWS, that can be automatically provisioned and workloads controlled by paying third-party clients, all through Amazon's self-service console.
 {: .fs-6 .fw-300 }

<span class="blue">This is essentially what HostJane is doing for our [web hosting customers](https://cloud.hostjane.com) under our hosting terms of service. This is why we align our [guarantee uptime](https://www.hostjane.com/legal/sla/) and refunds to Amazon's [Service Level Agreement](https://aws.amazon.com/legal/service-level-agreements/).</span>
{: .fs-6 .fw-300 }

A *private cloud*, on the other hand, usually tucked behind the firewall of a private company, is as Microsoft defines available: ["only to select users instead of the general public"](https://azure.microsoft.com/en-au/resources/cloud-computing-dictionary/what-is-a-private-cloud), and sometimes that means only those on the premises of the private cloud provider.
{: .fs-6 .fw-300 }

#  Limits on Hosting Support

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
