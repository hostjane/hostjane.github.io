---
layout: default
title: Managed cPanel / WHM VPS on Amazon EC2
parent: Managed VPS on EC2
description: How to host websites, email, and services with cPanel & WHM on AWS
nav_order: 2
permalink: /vps-hosting-tutorials/cpanel-whm/
---

# Managed cPanel/WHM on EC2 ![](/assets/wave.svg)
{: .fs-9 .no_toc }

[Buy your cPanel VPS](https://cloud.hostjane.com/vps/?appType=0&app=0){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [cPanel & WHM documentation](https://docs.cpanel.net/){: .btn .fs-5 .mb-4 .mb-md-0 }

It's fast and easy to get your full-managed VPS cPanel & WHM server up and running on Amazon EC2, we even set up your SSL certificate free. 
{: .fs-6 .fw-300 }

All you need to do is [point your domain](point-your-domain/) to the server.
{: .fs-6 .fw-300 }

<span class="purple">NB: cPanel can take up to 30-40 minutes to install on any server, so allow time for the server to send you the Admin password after purchase. Unlike our other services, it is not instant.</span>
{: .fs-6 .fw-300 }

<span class="blue">cPanel & WHM is licensed with an initial 2-week free trial license. You'll need to purchase a month license from cPanel directly to continue using cPanel on your Amazon EC2 server after the free trial expires.</span>
{: .fs-6 .fw-300 }

| Steps       | Actions required    | Time |
|:-------------|:------------------|
|   ![](/assets/one.svg)           | After purchase, login to the client area to see your **root password and IP address**. Amazon assigns a static IP address immediately, but your VPS will not be active until cPanel has finished installing. | Instant |

|   ![](/assets/two.svg)           | Wait 30 mins after purchase for your server to install cPanel and send your **cPanel Administrator username and password** to your email.| 30 - 40 minutes |
| ![](/assets/three.svg)  | Change your Administrator password  | 2 minutes |

| ![](/assets/four.svg) | [Point your domain](/point-your-domain/) to your hosting. Propagation usually takes less than 1 minute with Amazon Route 53 but can take much longer depending on your domain registrar.  | 1 minute |
| ![](/assets/five.svg)  | Authorize cPanel in set up. This can be done through any browser. Follow the steps to create a cPanel acount for your server to request cPanel sends you a 2 week trial license. | 5 minutes |
| ![](/assets/six.svg) | [Buy a license](https://www.cpanel.net/pricing/) from cPanel  | 2 minutes |

| ![](/assets/seven.svg)  | Request Simple Mail Transfer Protocol (SMTP) port 25 is unblocked. Like most cloud computing services, Amazon [blocks outbound traffic on Port 25](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-resource-limits.html#port-25-throttle) on all new EC2 servers. It's usually a formality to unblock the ports, but we will need to submit your use case to Amazon, so we can assist with that request | 2 minutes |

