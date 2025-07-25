---
layout: default
title: DirectAdmin VPS managed on EC2
parent: Managed VPS on EC2
description: DirectAdmin Tutorial
nav_order: 1
permalink: /vps-hosting-tutorials/directadmin/
---

# DirectAdmin VPS on EC2 ![](/assets/wave.svg)
{: .fs-9 .no_toc }

[Order your DirectAdmin VPS](https://cloud.hostjane.com/vps/?appType=0&app=1){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [DirectAdmin Docs](https://docs.directadmin.com/){: .btn .fs-5 .mb-4 .mb-md-0 }

[DirectAdmin](https://www.directadmin.com/) is a cheap, excellent entry-level web hosting control panel that offers most of the features you can find in cPanel. You'll need to already own or [purchase a new license](https://www.directadmin.com/pricing.php) from DirectAdmin to install our DirectAdmin VPS built and managed on bare-metal Amazon EC2 servers.
{: .fs-6 .fw-300 }
 
HostJane provides a free auto-renewing, SSL certificate matched to the domain or subdomain you provide in checkout.
{: .fs-6 .fw-300 }

<span class="blue">NB: DirectAdmin can take up to 40 mins to install on any server, so allow time for the server to send you the Admin password after purchase.</span>

| Steps       | Actions required    | Time |
|:-------------|:------------------|
|   ![](/assets/one.svg)          | Enter your [DirectAdmin license key](https://www.directadmin.com/pricing.php) in the [DirectAdmin VPS](https://cloud.hostjane.com/vps/?appType=0&app=1) checkout. Buy a new key from DirectAdmin if you do not own one. | 5 mins |

|   ![](/assets/two.svg)          | After purchase, login to the client area to see your **root password and IP address**. Amazon assigns a static IP address immediately, but your VPS will not be active until DirectAdmin has finished installing. | 40 mins |

| ![](/assets/three.svg)  | [Point your domain](/point-your-domain/) to your hosting. DirectAdmin requires 2 A-Records to be added at your domain registrar: "@" and "Server" in the hostname fields respectively.  | 1 min |

| ![](/assets/four.svg)  | Enable email. Log into your DirectAdmin control panel, navigate to "Email Manager," and then "Email Accounts." From there, click "Create Account" and enter the chosen username, password, and optional settings like quota and send limits. Review DirectAdmin [hostname documentation](https://docs.directadmin.com/other-hosting-services/email/perfect-email-setup.html). Port 2525, 587 and 465 are available for your use and satisfy most SMTP sending and receiving email requirements. Like most cloud computing services, Amazon [blocks outbound traffic on Port 25](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-resource-limits.html#port-25-throttle) on all new EC2 servers. We will need to submit your use case to AWS in case you wish to unblock Port 25. | 5 mins |