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

<span class="purple">NB: cPanel can take up to 50 minutes to install on any server, so allow time for the server to send you the Admin password after purchase. Unlike our other services, it is not instant.</span>
{: .fs-6 .fw-300 }

<span class="blue">cPanel & WHM is licensed with an initial 2-week free trial license. You'll need to purchase a month license from cPanel directly to continue using cPanel on your Amazon EC2 server after the free trial expires.</span>
{: .fs-6 .fw-300 }

| Steps       | Actions required    | Time |
|:-------------|:------------------|
|   ![](/assets/one.svg)           | After purchase, login to the client area to see your **root password and IP address**. Amazon assigns a static IP address immediately, but your VPS will not be active until cPanel has finished installing. | Instant |

|   ![](/assets/two.svg)           | Wait 50 mins after purchase for your server to install cPanel and send your **cPanel Administrator username and password** to your email. | 50 mins |
| ![](/assets/three.svg)  | Change your Administrator password  | 2 mins |

| ![](/assets/four.svg) | [Point your domain](/point-your-domain/) to your hosting. Propagation usually takes less than 1 min with Amazon Route 53 but can take much longer depending on your domain registrar.  | 1 min |
| ![](/assets/five.svg)  | Authorize cPanel in set up. This can be done through any browser. Follow the steps to create a cPanel acount for your server to request cPanel sends you a 2 week trial license. | 5 mins |
| ![](/assets/six.svg) | [Buy a license](https://www.cpanel.net/pricing/) from cPanel  | 2 mins |

| ![](/assets/seven.svg)  | Enable email. Follow the official [cPanel Mail Client set-up](https://docs.cpanel.net/cpanel/email/set-up-mail-client/) instructions. An "external mail client" refers to any email application, like Outlook, Thunderbird, or Spark. Port 2525, 587 and 465 are available for your use and satisfy most SMTP sending and receiving email requirements. Like most cloud computing services, Amazon [blocks outbound traffic on Port 25](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-resource-limits.html#port-25-throttle) on all new EC2 servers. We will need to submit your use case to AWS in case you wish to unblock Port 25. | 2 mins |

