---
layout: default
title: Amazon Linux 2023 VPS managed on EC2
parent: Managed VPS on EC2
description: Amazon Linux Tutorial
nav_order: 1
permalink: /vps-hosting-tutorials/amazon-linux/
---

# Amazon Linux VPS on EC2 ![](/assets/wave.svg)
{: .fs-9 .no_toc }

[Order your AL 2023 VPS](https://cloud.hostjane.com/vps/?appType=0&app=2){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [AL2023 information page](https://aws.amazon.com/linux/amazon-linux-2023/faqs/){: .btn .fs-5 .mb-4 .mb-md-0 }

[Amazon Linux 2023](https://aws.amazon.com/linux/amazon-linux-2023/) (AL2023), based on Fedora Linux and CentOS Stream, is Amazon's successor Linux distribution to Amazon Linux 2 with enhanced security features. 
{: .fs-6 .fw-300 }
 
HostJane provides a free auto-renewing, SSL certificate matched to the domain or subdomain you provide in checkout.
{: .fs-6 .fw-300 }

<span class="blue">Amazon Linux 2023 includes SELinux policy packages **selinux-policy** and **selinux-policy-targeted** by default.</span>

| Steps       | Actions required    | Time |
|:-------------|:------------------|
|   ![](/assets/one.svg)          | After purchase, login to the client area to see your **root password and IP address**. Amazon assigns a static IP address immediately, but your VPS will not be active until cPanel has finished installing. | Instant |

| ![](/assets/two.svg)  | [Point your domain](/point-your-domain/) to your hosting. Propagation usually takes less than 1 min with Amazon Route 53 but can take much longer depending on your domain registrar.  | 1 min |

| ![](/assets/three.svg)  | Request Simple Mail Transfer Protocol (SMTP) port 25 is unblocked. Like most cloud computing services, Amazon [blocks outbound traffic on Port 25](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-resource-limits.html#port-25-throttle) on all new EC2 servers. It's usually a formality to unblock the ports, but we will need to submit your use case to Amazon, so we can assist with that request | 2 mins |