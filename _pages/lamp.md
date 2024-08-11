---
layout: default
title: PHP (LAMP) on EC2
parent: Managed Cloud on EC2
description: Managed LAMP on Amazon EC2
nav_order: 2
permalink: /cloud-hosting/lamp-php/
---

# Managed LAMP on EC2 ![](/assets/wave.svg)
{: .fs-9 .no_toc }

[Buy LAMP VMs on AWS](https://cloud.hostjane.com/cloud/){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [LAMP Bitnami documentation](https://docs.bitnami.com/aws/infrastructure/lamp/){: .btn .fs-5 .mb-4 .mb-md-0 }

Run a [LAMP server](https://aws.amazon.com/what-is/lamp-stack/) (Linux; the web server, Apache; the database server, MySQL; and the programming language, PHP) with PHP-FPM on Amazon EC2, managed by HostJane's tech team.
{: .fs-6 .fw-300 }

<span class="green">Your LAMP server is [packaged by Bitnami](https://aws.amazon.com/marketplace/pp/prodview-6g3gzfcih6dvu) includes the latest releases of PHP and PHP-FPM, Apache, and MariaDB on Linux. It also includes phpMyAdmin, PHP main modules and Composer.</span>
{: .fs-6 .fw-300 }

| Steps       | Actions required    | Time |
|:-------------|:------------------|
|   ![](/assets/one.svg)          | After purchase, login to the client area to see your **root password and IP address**. Amazon assigns a static IP address immediately, but your VPS will not be active until the server configuration has finished installing. | Instant |

| ![](/assets/two.svg)  | [Point your domain](/point-your-domain/) to your hosting. Propagation usually takes less than 1 minute with Amazon Route 53 but can take much longer depending on your domain registrar.  | 1 minute |

| ![](/assets/three.svg)  | Request Simple Mail Transfer Protocol (SMTP) port 25 is unblocked. Like most cloud computing services, Amazon [blocks outbound traffic on Port 25](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-resource-limits.html#port-25-throttle) on all new EC2 servers. It's usually a formality to unblock the ports, but we will need to submit your use case to Amazon, so we can assist with that request | 2 minutes |