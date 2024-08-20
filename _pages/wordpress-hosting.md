---
layout: default
title: WordPress on EC2
description: Managed WordPress hosting docs and help tutorials
nav_order: 4
has_children: true
permalink: /wordpress-hosting/
---

Managed WordPress on Amazon EC2
{: .fs-9 .no_toc }

With a server team managing your WordPress virtual machine on [Amazon Elastic Compute Cloud](https://aws.amazon.com/ec2/) (EC2), the global leader in compute, server hardware and data, any WordPress site can scale like [WordPress VIP](https://wpvip.com/).
{: .fs-6 .fw-300 }

[Managed WordPress Hosting Plans](https://cloud.hostjane.com/wordpress/){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [Learn about Managed Amazon EC2](/cloud-hosting/){: .btn .fs-5 .mb-4 .mb-md-0 }

- [x] Managed [WordPress Multisite](hhttps://cloud.hostjane.com/wordpress)
- [x] Managed [WooCommerce](https://cloud.hostjane.com/wordpress)
- [x] Managed [Elementor](https://cloud.hostjane.com/wordpress)
- [x] Managed [Google Site Kit](https://cloud.hostjane.com/wordpress)
{: .fs-6 .fw-300 }

<iframe width="560" height="315" src="https://www.youtube.com/embed/q6WlzHLxNKI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

HostJane sets up your WordPress virtual machine on Amazon EC2 running the latest version of WordPress—[deployed by Bitnami](https://bitnami.com/stack/wordpress)—maps your EC2 instance to your domain or subdomain, assigns an Amazon elastic IP, and installs a free, auto-renewing SSL certificate. 
{: .fs-6 .fw-300 }

Your new Amazon WordPress cloud server will email you its admin username and password, within 3 minutes of the instance launching.
{: .fs-6 .fw-300 }

<span class="green">**Case Example:** HostJane automates in 2 minutes what [AWS Certified DevOps Engineer](https://aws.amazon.com/certification/certified-devops-engineer-professional/), Alok Kumar, manually does on the AWS terminal in 30 minutes, with added configurations, **on-going** 24/7 support and full server management.</span>
{: .fs-6 .fw-300 }

<iframe width="560" height="315" src="https://www.youtube.com/embed/5rlCUXjVaHE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

After 2-3 mins you'll get your WP-Admin password and must simply [point your domain to the IP address](/point-your-domain/) to see your new managed WordPress site in a web browser. 
{: .fs-6 .fw-300 }
 
 Advanced users should use an FTP like [Filezilla](https://filezilla-project.org/) or [CyberDuck](https://cyberduck.io/) to manage server files, and [PhPMyAdmin through this Bitnami tutiroial](https://docs.bitnami.com/aws/faq/get-started/access-phpmyadmin/) to you manage your WordPress database.
{: .fs-6 .fw-300 }

<span class="green">In addition to configuring the latest version of WordPress on your full-managed EC2 machine, HostJane offers Amazon EC2 instances with activated installations of the following software configured for reliability and speed.</span>

---

# Managed WordPress Hosting Set-Up

| Steps       | Actions required    | Time |
|:-------------|:------------------|
|   ![](/assets/one.svg)           | After purchase, login to the client area to see your **root password and IP address**. Amazon assigns a static IP address immediately, but your VPS will not be active until cPanel has finished installing. | Instant |

|   ![](/assets/two.svg)           | Wait 5 mins after purchase for your server to install cPanel and send your **WP-Admin username and password** to your email.| 5 minutes |
| ![](/assets/three.svg)  | Change your WP-Admin password  | 2 minutes |

| ![](/assets/four.svg) | [Point your domain](/point-your-domain/) to your hosting. Propagation usually takes less than 1 minute with Amazon Route 53 but can take much longer depending on your domain registrar.  | 1 minute |

| ![](/assets/five.svg)  | Request Simple Mail Transfer Protocol (SMTP) port 25 is unblocked. Like most cloud computing services, Amazon [blocks outbound traffic on Port 25](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-resource-limits.html#port-25-throttle) on all new EC2 servers. It's usually a formality to unblock the ports, but we will need to submit your use case to Amazon, so we can assist with that request | 2 minutes |

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
