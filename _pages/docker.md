---
layout: default
title: 1-Click Docker
parent: Cloud Computes
description: How to setup a Docker server
nav_order: 7
permalink: /cloud-compute/docker/
---

# 1-Click Docker

<span class="green">This tutorial helps you run the latest Docker version on HostJane cloud computes.
Docker can run on Ubuntu and CentOS.</span>

1. TOC
{:toc}

## 1. Get server IP and root password

After successful payment is approved, your server will be set up within 2 minutes.

### A. Login to the Hosting Portal

Bookmark login: [https://console.hostjane.com/client/login](https://console.hostjane.com/client/login)

In your Dashboard under Services, find your Docker server.

| Package | Label | Term  | Date Created | Date Renews | Options |
|:-------|:----------|:------|:----------|:------|:------|
| Docker | host.domain.com | 1 month @ $0.00 | Jan 1 | Feb 1 |*Manage* |

We offer 24×7×365 support

If you cannot see your Docker service, open a support case.

### B. Click the Manage option

This is the button in the last column under Services.

Here is the next screen that will display: 

| Package | Status|
|:-------|:----------|
| Docker | Active|
| **Label** | **Renew Date**|
| host.domain.com | Feb 1 |
| **Creation Date** | **Next Invoice**|
| Jan 1 | Feb 1 |
| **Billing Cycle** | **Recurring Amount**|
| 1 Month | $0.00 |

### C. Click *Statistics* in the side menu

| Field | Value |
|:-------|:----------|
| Main IP | 123.456.789.1 |
| Default password | demo123 |

The Main IP is your virtual machine's IP address.

The Default Password is the root password.

For security, HostJane does not send this to you by email.

You must login to your hosting account to review these credentials.

## 2. Login with SSH

Login to your server with PuTTY on Windows or an OpenSSH client in linux and MacOS devices:

```
docker run hello-world
```

The server will connect to Docker and download the latest image:

![](\assets\hosting\docker-hello-world.png)

## 3. The docker user

For security reasons, since it’s best not to run everyday administrative tasks as the root, we automatically create a docker user and docker group for you.

The docker user can run containers but has limited privileges.

You can switch to this user by typing the following on the command line:

```
su - docker
```

Add any other user to the docker group to run containers with that user.

<span class="orange">To find more information on running Docker containers, go to [Red Hat's guide](https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/7/html/7.0_release_notes/chap-red_hat_enterprise_linux-7.0_release_notes-linux_containers_with_docker_format).</span>

You now have the basic information to start using your new cloud server running Docker on your chosen Linux distribution.