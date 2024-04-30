+++
title = 'Homelab quickstart for free'
date = 2024-04-28
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

We are going to use CasaOS, a GUI for the Docker ecosystem, to set up a few essential services for your first homelab.
This is perfect for people just dipping their toes into homelabs since after some initial steps, we will be able to use CasaOS to set up services in an easy and visual way instead of command line code.
First start up your Windows computer and insert your USB drive.
We are going to install a tool called [Rufus](https://rufus.ie/en/) on this USB drive to be able to install a Linux operating system on your server.
So go ahead and open a web browser and navigate to the [Rufus homepage](https://rufus.ie/en/) and click on the Standard Windows x64 download.
Save the .exe file to whereever you like where you can find it again.
Open the file from your file explorer and Rufus should open up, no installation is necessary.

![Rufus screen](/images/homelab-quickstart/rufus.png)

Now all we need is an operating system to put on the USB drive.
I've chosen [Ubuntu Server](https://ubuntu.com/download/server#release-notes) since it is what I'm familiar with, but you can choose any of the available Linux distributions.
The Server part of Ubuntu Server just means that it won't have a GUI.
Which is perfect for our usecase since we will be using CasaOS for that.
[Download](https://ubuntu.com/download/server) a Ubuntu Server LTS version of your choice.
In Rufus select your USB stick under 'Device'.
Then from the SELECT button find your Ubuntu ISO file.
Leave everything else to default and click start.
You may be alerted that Rufus requires additional files to complete writing the ISO.
If this dialog box appears, select Yes to continue.
You will then be alerted that Rufus has detected that the Ubuntu ISO is an ISOHybrid image.
This means the same image file can be used as the source for both a DVD and a USB stick without requiring conversion.
Keep Write in ISO Image mode selected and click on OK to continue.
Rufus will also warn you that all data on your selected USB device is about to be destroyed.
This is a good moment to double check you’ve selected the correct device before clicking OK when you’re confident you have.
Wait until the Status bar at the bottom is fully green and says 'READY' and click 'CLOSE'.
We now have a USB stick that can install the Ubuntu Server operating system!

## Installing Ubuntu

Now it's time to insert the stick into your server and reboot the device.
It should recognise the installation media automatically during startup but you may need to hold down a specific key (usually F12, but the screen should show which one exactly) to bring up the boot menu and choose to boot from USB.
It will ususally look something like this.

![BIOS boot from usb](/images/homelab-quickstart/boot_bios.png)

Select your USB stick as the first option and find 'Save and exit', which should restart your server.
After some scrolling text, an image similar to this should appear.

![Ubuntu language select](/images/homelab-quickstart/ubuntu_language.png)

You can probably leave the keyboard configuration screen that is up next to the selected values.

The same goes for the next few screen where you select your install, networking, storage and filesystem setup. At the end you get an extra warning that you are about to delete all data on the disk that you will be using. So back out now if you have data on there that you want to keep.

You then need to input your name, the server's name, a username and password.

TODO: after this check which services need to be installed, probably ssh.

TODO: how to get ip address, note down

Some of these steps might be different for you, depending on the version of Ubuntu you are installing.
Don't be afraid and just read the prompts and decide what to select.

## Installing CasaOS

