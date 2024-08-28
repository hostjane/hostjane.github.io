---
layout: default
title: Multisite on Amazon EC2
parent: WordPress on EC2
description: How to migrate your WordPress site to HostJane VPS
nav_order: 3
permalink: /wordpress-hosting/multisite/
---

# Managed WP Multisite on EC2 ![](/assets/wave.svg)
{: .fs-9 .no_toc }

[Buy WordPress Multisite VMs on AWS](https://cloud.hostjane.com/vps/?appType=0&app=2){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [Multsite documentation](https://developer.wordpress.org/advanced-administration/multisite/prepare-network/){: .btn .fs-5 .mb-4 .mb-md-0 }

[WordPress Multisite](https://developer.wordpress.org/advanced-administration/multisite/) is designed to host multiple blog websites on one instance of WordPress. 
{: .fs-6 .fw-300 }

When you add new blog websites to your WordPress Multisite, you can configure them to use their own domains or a subdomain of your WordPress Multisite's primary domain.
{: .fs-6 .fw-300 }

<span class="blue">Note that HostJane will configure your free auto-renewing SSL certificate to your **primary domain** provided in checkout.</span>

| Steps       | Actions required    | Time |
|:-------------|:------------------|
|   ![](/assets/one.svg)           | After purchase, login to the client area to see your **root password and IP address**. Amazon assigns a static IP address immediately, but your VPS will not be active until WordPress has finished installing. | Instant |

|   ![](/assets/two.svg)           | Wait 5 mins after purchase for your server to install WordPress and send your **WP-Admin username and password** to your email.| 5 mins |
| ![](/assets/three.svg)  | Change your WP-Admin password  | 2 mins |

| ![](/assets/four.svg) | [Point your domain](/point-your-domain/) to your hosting. Propagation usually takes less than 1 min with Amazon Route 53 but can take much longer depending on your domain registrar. | 1 min |

| ![](/assets/five.svg)  | Request Simple Mail Transfer Protocol (SMTP) port 25 is unblocked. Like most cloud computing services, Amazon [blocks outbound traffic on Port 25](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-resource-limits.html#port-25-throttle) on all new EC2 servers. It's usually a formality to unblock the ports, but we will need to submit your use case to Amazon, so we can assist with that request | 2 mins |