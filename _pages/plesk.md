---
layout: default
title: Managed Plesk VPS on Amazon EC2
parent: Managed VPS on EC2
description: How to Install and Setup Plesk on your VPS Server
nav_order: 3
permalink: /vps-hosting-tutorials/plesk/
---

# Plesk VPS on EC2 ![](/assets/wave.svg)
{: .fs-9 .no_toc }

[Buy your Plesk VPS](https://cloud.hostjane.com/vps/?appType=0&app=2){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [Plesk documentation](https://support.plesk.com/hc/en-us){: .btn .fs-5 .mb-4 .mb-md-0 }

It's fast and easy to get your full-managed VPS Plesk server up and running on Amazon EC2, we even set up your SSL certificate free.
{: .fs-6 .fw-300 }

All you need to do is [point your domain](point-your-domain/) to the server.
{: .fs-6 .fw-300 }

<span class="blue">NB: Plesk can take up to 50 mins to install on any server, so allow time for the server to send you the Admin password after purchase.</span>
{: .fs-6 .fw-300 }

![](/assets/plesk-screenshot.png)

<span class="orange">Plesk now requires users to own an existing license key or [purchase a new license from Plesk directly](https://www.plesk.com/pricing/) per server.</span>
{: .fs-6 .fw-300 }

| Steps       | Actions required    | Time |
|:-------------|:------------------|
|   ![](/assets/one.svg)     | After purchase, login to the client area to see your **root password and IP address**. Amazon assigns a static IP address immediately, but your VPS will not be active until cPanel has finished installing. | Instant |

|   ![](/assets/two.svg) | Wait 20-30 mins after purchase for your server to install Plesk and send your **on-time Plesk URL** to your email.| 30 mins |

| ![](/assets/three.svg) | Change your Administrator password  | 2 mins |
| ![](/assets/four.svg) | [Point your domain](/point-your-domain/) to your hosting. Propagation usually takes less than 1 min with Amazon Route 53 but can take much longer depending on your domain registrar.  | 1 min |
| ![](/assets/five.svg)| [Buy a license](https://www.plesk.com/pricing/) from Plesk  | 2 mins |

| ![](/assets/six.svg) | Enable email. Follow the official [Plesk Mail Client set-up](https://docs.plesk.com/en-US/obsidian/customer-guide/quick-start-with-plesk/set-up-mail-accounts/1-create-mail-account.69277/) and [Server Wide Mail Setting](https://docs.plesk.com/en-US/obsidian/administrator-guide/mail/configuring-serverwide-mail-settings.59430/) instructions. To access your mailbox, you'll generally need an external mail client" like Outlook, Thunderbird, or Spark.  | 3 mins |

| ![](/assets/seven.svg) | Email Ports. Port 2525, 587 and 465 are available for your use and satisfy most SMTP sending and receiving email requirements. Like most cloud computing services, Amazon [blocks outbound traffic on Port 25](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-resource-limits.html#port-25-throttle) on all new EC2 servers. We will need to submit your use case to AWS in case you wish to unblock Port 25. | 2 mins |