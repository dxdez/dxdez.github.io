---
layout: post
title:  "Linux Handbook, VPN OpenConnect & Extras"
date:   2024-04-22 11:26:24 -0500
---

### Articles

This is a series of blog posts about creating modular worlds with tilemaps in the Phaser 3 game engine.

- [Using Docker to Set up Nginx Reverse Proxy With Auto SSL Generation](https://linuxhandbook.com/nginx-reverse-proxy-docker/ "Using Docker to Set up Nginx Reverse Proxy With Auto SSL Generation")
- [Updating Docker Containers With Zero or Minimum Downtime](https://linuxhandbook.com/update-docker-container-zero-downtime/ "Updating Docker Containers With Zero or Minimum Downtime")
- [Container Management With Podman](https://linuxhandbook.com/podman/ "Container Management With Podman")

### Source - Linux Handbook

The original site for both posts can be found here: [Linux Handbook](https://linuxhandbook.com/ "Linux Handbook"). The link is also included under the Linux resource page. 

### VPN Open Connect

To connect to a VPN endpoint from the Linux terminal using your username and password, you can follow these steps. First, install the OpenConnect VPN client on your Linux machine:
```
sudo apt-get install openconnect
```

Then, use the openconnect command to initiate the VPN connection, providing the VPN endpoint URL and your username:
```
sudo openconnect connect.whatever.com --user=YOUR_USERNAME
```

Replace YOUR_USERNAME with your actual username for the VPN.

### The cloud is over-engineered and overpriced

This is a video on setting up hosting using linux, git and docker. The solution involves creating a build using NixOS and creating a basic configuration with git, docker, ssh and other needed tools. The purpose is to create an alternative from a full cloud solution. The video can be found [here](https://www.youtube.com/watch?v=jFrGhodqC08 "here").
