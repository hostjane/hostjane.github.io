---
layout: default
title: Nginx on Amazon EC2
parent: Managed Cloud on EC2
description: Managed Nginx on Amazon EC2
nav_order: 3
permalink: /cloud-hosting/nginx/
---

# Managed Nginx on EC2 ![](/assets/wave.svg)
{: .fs-9 .no_toc }

[Buy NGINX VMs on AWS](https://cloud.hostjane.com/cloud/){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [NGINX Bitnami documentation](https://bitnami.com/stack/nginx){: .btn .fs-5 .mb-4 .mb-md-0 }

NGINX, said as *Engine-x*, is an open-source web server and pre-configured LEMP stack which includes Linux, Nginx, MySQL, and PHP; ready to run your code. NGINX is mainly used as a web server to serve static content like HTML, CSS and images. The LEMP stack includes other components and libraries such as phpMyAdmin, SQLite, ImageMagick, FastCGI, Memcache, GD, CURL, PEAR, PECL and Composer.
{: .fs-6 .fw-300 }

NGINX can also be used as a *Reverse Proxy* for security and scaling to forward client requests to other servers; for *HTTP Caching*; and for *Load Balancing*, to route incoming traffic to different servers to improve performance.
{: .fs-6 .fw-300 }

<span class="blue">NGINX on Amazon EC2, [packaged by Bitnami](https://aws.amazon.com/marketplace/pp/prodview-lzep7hqg45g7k), is a light-weight, stable and high-performance web server to serve your website or app's content.</span>
{: .fs-6 .fw-300 }

<span class="green">Managed by HostJane from Debian server set-up to root password allocation, let our admins take care of your NGINX virtual machine for you while it runs on Amazon's infrastructure.</span>
{: .fs-6 .fw-300 }

| Steps       | Actions required    | Time |
|:-------------|:------------------|
|   ![](/assets/one.svg)          | After purchase, login to the client area to see your **root password and IP address**. Amazon assigns a static IP address immediately, but your VPS will not be active until the server configuration has finished installing. | Instant |

| ![](/assets/two.svg)  | [Point your domain](/point-your-domain/) to your hosting. Propagation usually takes less than 1 minute with Amazon Route 53 but can take much longer depending on your domain registrar.  | 1 minute |

| ![](/assets/three.svg)  | Request Simple Mail Transfer Protocol (SMTP) port 25 is unblocked. Like most cloud computing services, Amazon [blocks outbound traffic on Port 25](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-resource-limits.html#port-25-throttle) on all new EC2 servers. It's usually a formality to unblock the ports, but we will need to submit your use case to Amazon, so we can assist with that request | 2 minutes |