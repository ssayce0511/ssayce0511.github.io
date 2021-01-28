---
layout: post
title: Open Source Reflections
subtitle: Reflections on Open Source in Today's World
tags: [reading, reflection, open-source]
---
For this blog post, I read two articles from [this website](https://opensource.com/article/20/12/containers-101) and will share what I learned and my reflections on the articles. 

## 6 Container concepts you need to know 

This [article](https://opensource.com/article/20/12/containers-101) summarized what containers were, which is something I'm not totally familar with. Containers are similar to VM's, and currently they are being used as a complementary system to VM's rather than a competitor. Essentially, a container is an application bundle of lightweight components, such as application dependencies, libraries, and configuration files, that run in an isolated environment on top of traditional operating systems or in virtualized environments for easy portability and flexibility. 

![Diagram](https://opensource.com/sites/default/files/uploads/container_architecture.png)

The figure above shows the structure of a container. 

Containers have their advantages, they are more flexible than VM's. They also create a common set of building blocks that can be reused in development at any stage so you can re-create environments for deployment. Docker revolutionized containers and caused them to become more popular. Compared to virtualization, containers make it simpler to achieve flexibility, consistency, and the ability to deploy applications faster—the main principles of DevOps.

In terms of my personal learning, I wasn't aware of what containers were before reading this article and now I have a better understanding of how they function. I am familiar with VMs and have used them before and I had heard of Docker but never really knew what was going on. This article summarized all the necessary information. 

## US government accelerating development and release of open source

This [article](https://opensource.com/government/14/4/interview-david-wheeler) interviews David Wheeler, a long time leader and advisor to the US government related to open source software issues. In the article Wheeler describes the current state of OS software in the government as improving. There are many smaller OS components used throughout their systems. The source of the problem is that it is still common for acquisitions to ignore OSS. 

Wheeler goes on to explain how in the eyes of the law, nearly all OSS can be labeled as commerical software, since it has non-government use and is licensed to the public. Law requires acquisitioners to examine all alternatives, and even value commercial options higher. Because of this misconception about OSS they are inadverdently breaking the law by not looking at open source as an option. 

Forking projects is still a big issue, Wheeler states. Contractors typically get paid far more if they can convince the government that the software must be rewritten from scratch or must at least be changed and maintained "specially" in a way that will cause the government to pay for all future changes. Government employees who are officially managing the project may be smart in general, but they often know little about software. Obviously, managers who don’t understand what they’re managing are often easily fooled. Part of the problem is that in most agencies, the easy thing to do is to create project-special forks, even though it is almost always the highest-cost and highest-risk approach for maintenance. 

Looking towards the future, Wheeler is excited about the OSS that the government is releasing lately. The White House not only uses Drupal, but has released many improvements it’s made. For example, the White House improved Drupal’s accessibility; by releasing that improvement they have probably helped millions of disabled people around the world.

Reflecting on this article, I learned a lot about the governmental policies surrounding OSS. You would assume OSS makes everything simple, but it is obviously anything but according to David Wheeler. Personally I think shifting towards OSS is smart for the government and is an efficent way to save money and resources, if they play the game correctly and have informed managers. 

