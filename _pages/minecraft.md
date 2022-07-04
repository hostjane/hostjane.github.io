---
layout: default
title: 1-Click Minecraft
parent: Cloud Computes
description: How to setup a LAMP server
nav_order: 8
permalink: /cloud-compute/minecraft/
---

This is a legacy article and no longer updated
HostJane offers basic Minecraft servers with no pre-installed modules.

Download Minecraft for Windows or MacOS devices then connect to your server through the game client to start playing.
Please note that by running a Minecraft server here, you’re telling us that you agree to Mojang AB’s End User Licensing Agreement (EULA).
1. Get server IP and root password
After successful payment is approved, your server will be set up within 2 minutes.

A. Login to the Hosting Portal
Bookmark login: https://console.hostjane.com/client/login

In the Dashboard under Services, look for the Minecraft server you have provisioned.


We offer 24×7×365 support

If you cannot see your service, open a support case.

B. Click Manage next to the Minecraft server item
You will be transferred to the server’s dashboard.


C. Click Statistics in the menu
Below is a sample screenshot of the Server Information.


In this example, the server link is: https://123.456.789.1:25565

In this example case the IP is: 123.456.789.1

Your Server Link
https://[Your_Server’s_IP]/:25565
For security, HostJane does not send this to you by email.

You must login to your hosting account to review these credentials.

2. Connect to your server in Minecraft
In the Minecraft game client:

Click Multiplayer

Then click Direct Connect

Type out:

[Your_Server’s_IP]:25565
Replace Your Server’s IP with your Minecraft server’s IP as found in Statistics

Next, click Join Server to begin play.

Minecraft is resource intensive. As your player count increases you may need to scale to a bigger cloud server.

3. Login with SSH to your server
Login to your server with PuTTY on Windows or an OpenSSH client in linux and MacOS devices:

ssh -l root [Your_Server's_IP]
Replace Your_Server’s_IP with the server IP address given in Statistics.

4. Connect to the game console
screen -r
You can type commands here.

To exit:

ctrl + A then type d

To establish system status and other housekeeping actions, use systemctl

For example:

systemctl status minecraft.service
On an active, properly configured Minecraft server you should get this response:



To launch Minecraft use:

/home/minecraft/minecraft_server.sh
Restart the server as root user after making any edits to minecraft_server.sh.

systemctl restart minecraft.service
To stop your Minecraft server, enter:

systemctl stop minecraft.service