---
layout: post
title:  "Improving version management of dev-tools on Linux"
date:   2020-02-27 23:21:59 -0300
categories: ideias
---

#### Why is development tool version management so often difficult?
If you've ever needed to maintain multiple projects developed in different technologies with different language and framework versions. So, you know how much   it's complicated to manage everything on the same machine.

#### But the packaging tools of Linux distributions (like Ubuntu's apt), they have this mission, don't they? 
They work for stable tools, like the JDK (Java Development Kit), which are not updated frequently.

If you want to use unstable versions or tools that change frequently, packaging tools are not a good option, although it also doesn't solve the problem of installing more than one version of the same tool (for example: two versions of nodejs).

#### Most common issues with managing versions of development tools:
* Services installation and configuration
* Many different places to download installers
* time spent installing and configuring a development environment
* Organization (directory tree)
* PATH configuration for different versions of the same tool

#### For services version management there is an obvious solution: Docker
Using Docker, you can easily activate and deactivate any type of service when necessary to easily manage different versions of a specific service (for example: different versions of postgres).
Another big advantage is the fact that the images of the main services needed are in DockerHub (which makes it easy to find) and, with a reasonable knowledge of docker technology, you can quickly create scripts to create and run containers organized in a single location (where you can take them to another computer or just make a backup).

be continue ... 
