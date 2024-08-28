---
layout: default
title: Windows & SQL Server on Amazon EC2
parent: Managed Cloud on EC2
description: Managed Windows on Amazon EC2
nav_order: 6
permalink: /cloud-hosting/windows-hosting/
---

# Managed Windows Server on EC2 ![](/assets/wave.svg)
{: .fs-9 .no_toc }

[Run Windows Server VMs on AWS](https://cloud.hostjane.com/windows/){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [Windows Server EC2 documentation](https://aws.amazon.com/marketplace/pp/prodview-dq4sxno5vuy7m){: .btn .fs-5 .mb-4 .mb-md-0 }

Configured for Amazon EC2, [Windows Server](https://aws.amazon.com/windows/products/ec2/) and [SQL Server](https://docs.aws.amazon.com/sql-server-ec2/latest/userguide/sql-server-on-ec2-overview.html), managed by HostJane's tech team enables you to deploy Windows-based applications for website and web service, data processing, distributed testing, ASP.NET application hosting, using the Microsoft Web Platform.
{: .fs-6 .fw-300 }

<span class="blue">Connect to your Windows machine by Remote Desktop Connection (RDC) which uses the [Remote Desktop Protocol](https://learn.microsoft.com/en-us/troubleshoot/windows-server/remote/understanding-remote-desktop-protocol) (RDP).</span>
{: .fs-6 .fw-300 }

| Steps       | Actions required    | Time |
|:-------------|:------------------|
|   ![](/assets/one.svg)          | After purchase, login to the client area to see your **root password and IP address**. Amazon assigns a static IP address immediately, but your VPS will not be active until the server configuration has finished installing. | Instant |

| ![](/assets/two.svg)  | [Point your domain](/point-your-domain/) to your hosting. Propagation usually takes less than 1 min with Amazon Route 53 but can take much longer depending on your domain registrar.  | 1 min |

| ![](/assets/three.svg)  | Request Simple Mail Transfer Protocol (SMTP) port 25 is unblocked. Like most cloud computing services, Amazon [blocks outbound traffic on Port 25](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-resource-limits.html#port-25-throttle) on all new EC2 servers. It's usually a formality to unblock the ports, but we will need to submit your use case to Amazon, so we can assist with that request | 2 mins |
