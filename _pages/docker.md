---
layout: default
title: 1-Click Docker
parent: Cloud Computes
description: How to setup a LAMP server
nav_order: 7
permalink: /cloud-compute/docker/
---

This tutorial helps you run the latest Docker version on HostJane cloud computes.
Docker can run on Ubuntu and CentOS.

1. Get server IP and root password
After successful payment is approved, your server will be set up within 2 minutes.

A. Login to the Hosting Portal
Bookmark login: https://console.hostjane.com/client/login

In the Dashboard under Services, look for the Docker server you have provisioned.


We offer 24×7×365 support

If you cannot see your service, open a support case.

B. Click Manage next to the Docker server item
You will be transferred to the server’s dashboard.


C. Click Statistics in the menu
Below is a sample screenshot of the Server Information.


The Main IP is your virtual machine's IP address.

The Default Password is the root password.

For security, HostJane does not send this to you by email.

You must login to your hosting account to review these credentials.

2. Login with SSH
Login to your server with PuTTY on Windows or an OpenSSH client in linux and MacOS devices:

docker run hello-world

The server will connect to Docker and download the latest image:


3. The docker user
For security reasons, since it’s best not to run everyday administrative tasks as the root, we automatically create a docker user and docker group for you.

The docker user can run containers but has limited privileges.

You can switch to this user by typing the following on the command line:

su - docker

Add any other user to the docker group to run containers with that user.

To find more information on running Docker containers, go to Red Hat’s guide.
You now have the basic information to start using your new cloud server running Docker on your chosen Linux distribution.