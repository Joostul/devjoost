+++
title = 'What is a homelab?'
date = 2024-04-25
draft = true
categories = ['Development','Servers']
series = ['Homelab']
tags = ['Homelab','Home Server','Servers','Personal Experience','Hardware','Selfhosting']
+++

## Introduction

The definition of a homelab is straight forward; it is a lab environment that you run at home.
In the context of development, a lab is a place where you can safely do experiments.
In my case, I wanted to learn more about Kubernetes from scratch and thus set up a few servers at my home.

## Why should I want a homelab?

As mentioned, in your homelab you can experiment with all the things you want to learn more about or get experience with using without worrying about all the extra complexity that comes with office or workplace environments.
It can very easily become a place that is constantly growing and expanding based on learning what other services and projects are possible.
For example, I had never heard about blocking ads by running your own DNS server in [Pi-hole](https://pi-hole.net/).
I am also running a service called [Tandoor](https://tandoor.dev/)(self-hosted instructions [here](https://docs.tandoor.dev/install/docker/)), so we can keep track of our favorite recipes and even plan our meals and grocery lists.
Another very useful addition is a storage pool which is accessible to any PC in the house using Samba shares.

## What hardware should I use?

You can use any hardware that you want.
Anything from an old PC or laptop that you have lying around, to a full server rack with a UPS or a single Raspberry Pi.
The fun part of a homelab is that you can start small and add or replace parts as you go.

![Different homelabs](/images/what-is-homelab/homelab_hardware.png)

## What else can I do with it?

Since a server is just a PC, you can do just about anything on it.
That said, some common scenarios are:

* Running a game server, for example, a Minecraft server that your kids (or you) and your friends can play on together.
* Storage, for example, a NAS (Network Attached Storage).
* Media management, for example, organize your photos or watch movies and TV shows.
* Get experience with using different operating systems like Linux or Windows in virtualized environments.
* Automate processes, for example sending emails at a set time and creating backups of certain files.
* Home automation, like turning off or on lights or heating at certain times.
* Host a website or service for you or anyone to use.

There are many more use cases and a good place to check if you want a comprehensive list is the [awesome selfhosted](https://github.com/awesome-selfhosted/awesome-selfhosted) GitHub page.

## How do I set this all up?

You can use any machine you want; most things are possible on most operating systems.
When you are using an old Windows PC or laptop it is easy to set up [Docker](https://www.docker.com/) and start running services.
This might be an advisable first step if you are not in the IT space or don't know what an IP address is.
However, for IT people, especially if you are a little bit more familiar with Linux, I would advise setting up a Hypervisor like [Proxmox](https://www.proxmox.com/en/) or [UNRAID](https://unraid.net/).
I am currently using Proxmox so look forward to future posts on that topic.

Have fun and don't be afraid!
