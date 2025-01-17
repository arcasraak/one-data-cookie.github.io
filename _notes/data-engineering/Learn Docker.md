---
title: Learn Docker
title-cs: 
category: data-engineering
tags: [docker]
season: autumn
created: 13 Dec 2021
updated: 23 Aug 2022
sources: Misc
---

## Intro
- [The Missing Semester](https://missing.csail.mit.edu/2020/qa/):
> *What is the difference between Docker and a Virtual Machine?*
> 
> Docker is based on a more general concept called containers. The main difference between containers and virtual machines is that virtual machines will execute an entire OS stack, including the kernel, even if the kernel is the same as the host machine. Unlike VMs, containers avoid running another instance of the kernel and instead share the kernel with the host. In Linux, this is achieved through a mechanism called LXC, and it makes use of a series of isolation mechanisms to spin up a program that thinks it’s running on its own hardware but it’s actually sharing the hardware and kernel with the host. Thus, containers have a lower overhead than a full VM. On the flip side, containers have a weaker isolation and only work if the host runs the same kernel. For instance if you run Docker on macOS, Docker needs to spin up a Linux virtual machine to get an initial Linux kernel and thus the overhead is still significant. Lastly, Docker is a specific implementation of containers and it is tailored for software deployment. Because of this, it has some quirks: for example, Docker containers will not persist any form of storage between reboots by default.


- [Docker Hub](https://hub.docker.com/)
- [Tutorial](https://docs.docker.com/get-started/)