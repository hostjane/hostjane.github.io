---
layout: default
title: Elementor Website Builder on Amazon EC2
parent: WordPress on EC2
description: How to migrate your WordPress site to HostJane VPS
nav_order: 2
permalink: /wordpress-hosting/elementor/
---

# Managed Elementor on EC2 ![](/assets/wave.svg)
{: .fs-9 .no_toc }

[Buy Elementor VMs on AWS](https://cloud.hostjane.com/vps/?appType=0&app=2){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [Elementor documentation](https://elementor.com/help/){: .btn .fs-5 .mb-4 .mb-md-0 }

[Elementor Website Builder](https://elementor.com/) is tailored to launch activated on top of a fast WordPress virtual machine configured for speed and WordPress requirements. 
{: .fs-6 .fw-300 }

HostJane provides a free auto-renewing, SSL certificate matched to the domain or subdomain you provide in checkout.
{: .fs-6 .fw-300 }

| Steps       | Actions required    | Time |
|:-------------|:------------------|
|   ![](/assets/one.svg)           | After purchase, login to the client area to see your **root password and IP address**. Amazon assigns a static IP address immediately, but your VPS will not be active until WordPress has finished installing. | Instant |

|   ![](/assets/two.svg)           | Wait 5 mins after purchase for your server to install WordPress and send your **WP-Admin username and password** to your email.| 5 mins |
| ![](/assets/three.svg)  | Change your WP-Admin password  | 2 mins |

| ![](/assets/four.svg) | [Point your domain](/point-your-domain/) to your hosting. Propagation usually takes less than 1 min with Amazon Route 53 but can take much longer depending on your domain registrar. | 1 min |

| ![](/assets/five.svg)  | Enable email. You'll need to sign up for a 3rd party transactional mail provider. We recommend you activate these plugins: [Mail Gun for WordPress](https://wordpress.org/plugins/mailgun/) or [Brevo](https://wordpress.org/plugins/mailin/) or use a free compatible SMTP plugin like [WP Mail SMTP](https://wordpress.org/plugins/wp-mail-smtp/) or [Post SMTP](https://wordpress.org/plugins/post-smtp/) for Gmail or email services that don’t offer their own plugin. If you need to send an email blast, we recommend you activate [MailChimp](https://wordpress.org/plugins/mailchimp-for-wp/), Brevo, or [Constant Contact](https://wordpress.org/plugins/constant-contact-forms/). | 5 mins |

| ![](/assets/six.svg)  | Email Ports. Port 2525, 587 and 465 are available for your use and satisfy most SMTP sending and receiving email requirements. Like most cloud computing services, Amazon [blocks outbound traffic on Port 25](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-resource-limits.html#port-25-throttle) on all new EC2 servers. We will need to submit your use case to AWS in case you wish to unblock Port 25. | 2 mins |