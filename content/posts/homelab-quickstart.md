+++
title = 'Homelab quickstart for 0 euros'
date = 2024-04-27
draft = false
categories = ['Development','Servers']
series = ['Homelab']
tags = ['Homelab','Home Server','Linux','Walkthrough','Hardware','level100']
+++

## Introduction

In the last post I talked about a homelab and what it really is.
If that tickled your fancy and you want to get started, but you don't have much developer or even Linux experience, this is the post for you!
We will talk about how to set up your very own homelab to get you started with basically zero costs, given you have some basic things laying around.
What you will need is:

* An old computer (could be a PC or laptop, or anything really) that you don't use anymore (this will be your server)
* A USB stick (4GB or larger)

You also kind of need  a PC that you do use, since we are going to access our homelab computer from a web Graphical User Interface (GUI).

## Getting started

I'm going to assume you are using windows for your operating system since that makes this walkthrough quite a bit easier.
I personally don't have experience with macOS and if you're already on Linux, you presumeably don't need this walkthrough :smile:.

If the computer you are using is too old, you might run into problems later down the line.
I have not experienced this myself, but I assume not everyone following this walkthrough will get through it without any problems.
If you encounter any problems that you just can't find a way to get around, feel free to reach out.

## Actually getting started

We are going to use CasaOS, a GUI, to set up a few essential services for your first homelab.
This is perfect for people just dipping their toes into homelabs since after some initial steps, we will be able to use CasaOS to set up services in an easy and visual way instead of command line code.
First start up your Windows computer and insert your USB drive.
We are going to install a tool called [Rufus](https://rufus.ie/en/) on this USB drive to be able to install a Linux operating system on your server.
So go ahead and open a web browser and navigate to the [Rufus homepage](https://rufus.ie/en/) and click on the Standard Windows x64 download.
Save the .exe file to whereever you like where you can find it again.
Open the file from your file explorer and Rufus should open up, no installation is necessary.
