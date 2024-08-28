---
layout: default
title: Server troubleshooting
description: Quick fixes for common hosting issues
nav_order: 3
permalink: /hosting-troubleshooting/
---

# Answers for common issues ![](/assets/wave.svg)
{: .fs-9 .no_toc }

Note: HostJane sells Amazon EC2 servers that we manage for people, not domain names. DNS propagation issues and problems with A-Records are often best addressed at your domain registrar. For all server-related issues, we may have answered your question below.
{: .fs-6 .fw-300 }

## 5 Minute Read
{: .no_toc .text-delta }

1. TOC
{:toc}

## I haven't got my IP or server email yet?

If you paid for a managed cPanel or Plesk Amazon EC2 server, it takes up to 40 minutes for cPanel and up to 30 mins for Plesk to finish installing on any new server. Your virtual machine is configured to send you the IP address and login credentials after installation is complete.
{: .fs-6 .fw-300 }

<span class="yellow">If you paid for a linux VPS, WordPress virtual machine, linux cloud or windows server and have not received your server email after 5 mins, please [contact us](https://www.hostjane.com/marketplace/contact) without delay.</span>
{: .fs-6 .fw-300 }

## Why is the SSL certificate showing as unsecure?

Bear in mind DNS propagation can take a lot longer in some global regions, and it may take more time. This is also the case if you have updated A-records recently on the same domain, there can be a resulting [DNS cache issue](https://www.whatsmydns.net/flush-dns.html). After waiting at least 30 mins, test your SSL certificate using [Qualys SSL Lab Test](https://www.ssllabs.com/ssltest/) and [SSL Shopper](https://www.sslshopper.com/ssl-checker.html).
{: .fs-6 .fw-300 } 

<span class="green">If you are still seeing an issue after 30 mins or your SSL test results fail to clear, please [contact us](https://www.hostjane.com/marketplace/contact) without delay.</span>

## Why is SSH not working on my server?

If you have verified the IP address and your keys are correct, and you have not set up or changed any of the ports on your server's firewall, please [contact us](https://www.hostjane.com/marketplace/contact) without delay.
{: .fs-6 .fw-300 }

