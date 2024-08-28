---
layout: default
title: Laravel on Amazon EC2
parent: Managed Cloud on EC2
description: Managed Laravel virtual machine on Amazon EC2
nav_order: 1
permalink: /cloud-hosting/laravel/
---

# Managed Laravel on EC2 ![](/assets/wave.svg)
{: .fs-9 .no_toc }

[Buy Laravel VMs on AWS](https://cloud.hostjane.com/cloud/){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [Laravel documentation](https://laravel.com/docs){: .btn .fs-5 .mb-4 .mb-md-0 }

Use Amazon EC2 virtual machines perfected [for Laravel](https://laravel.com/)—the open-source PHP web framework best for *PHP web application* development—compiled and configured by a professional tech team. Your Laravel server will deliver your Laravel database credentials, by email, instantly on provisioning.
{: .fs-6 .fw-300 }

<span class="blue">Your Laravel Amazon EC2 machine includes a free, auto-renewing SSL certificate matched to the domain you provide in checkout.</span>
{: .fs-6 .fw-300 }

| Steps       | Actions required    | Time |
|:-------------|:------------------|
|   ![](/assets/one.svg)          | After purchase, login to the client area to see your **root password and IP address**. Amazon assigns a static IP address immediately, but your VPS will not be active until the server configuration has finished installing. | Instant |

| ![](/assets/two.svg)  | [Point your domain](/point-your-domain/) to your hosting. Propagation usually takes less than 1 min with Amazon Route 53 but can take much longer depending on your domain registrar.  | 1 min |

| ![](/assets/three.svg)  | Your Laravel database information including Laravel database name, user and password and the MySQL Root password is sent by the server to the purchaser's account email.  | 3-4 mins |

| ![](/assets/four.svg)  | Request Simple Mail Transfer Protocol (SMTP) port 25 is unblocked. Like most cloud computing services, Amazon [blocks outbound traffic on Port 25](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-resource-limits.html#port-25-throttle) on all new EC2 servers. It's usually a formality to unblock the ports, but we will need to submit your use case to Amazon, so we can assist with that request | 2 mins |