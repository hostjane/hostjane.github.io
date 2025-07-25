---
layout: default
title: Django on Amazon EC2
parent: Managed Cloud on EC2
description: Managed Django virtual machine on Amazon EC2
nav_order: 4
permalink: /cloud-hosting/django/
---

# Managed Django on EC2 ![](/assets/wave.svg)
{: .fs-9 .no_toc }

[Run Django VMs on AWS](https://cloud.hostjane.com/vps/?appType=0&app=2){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [Django documentation](https://docs.djangoproject.com/){: .btn .fs-5 .mb-4 .mb-md-0 }

Django is a python-based web framework perfect for fast, secure content management systems, wikis, social networking and blogging that [can deliver content](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Introduction) in almost any format (including HTML, RSS feeds, JSON, and XML).
{: .fs-6 .fw-300 }

| Steps       | Actions required    | Time |
|:-------------|:------------------|
|   ![](/assets/one.svg)          | After purchase, login to the client area to see your **root password and IP address**. Amazon assigns a static IP address immediately, but your VPS will not be active until the server configuration has finished installing. | Instant |

| ![](/assets/two.svg)  | [Point your domain](/point-your-domain/) to your hosting. Propagation usually takes less than 1 min with Amazon Route 53 but can take much longer depending on your domain registrar.  | 1 min |

| ![](/assets/three.svg)  | Email Ports. Port 2525, 587 and 465 are available for your use and satisfy most SMTP sending and receiving email requirements. Like most cloud computing services, Amazon [blocks outbound traffic on Port 25](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-resource-limits.html#port-25-throttle) on all new EC2 servers. We will need to submit your use case to AWS in case you wish to unblock Port 25. | 2 mins |