---
title: "Debian The Bad"
date: 2024-09-06T03:22:41+02:00
author: "emilio.red"
description: "My opinion on using Debian and its features."
draft: false
---
Hello everyone, today I will be sharing my thoughts and opinions on the Debian operating system.

# Debian

Debian is a GNU/Linux operating system that stands out for its incredible stability, security and performance. So much so that many Linux distributions are based on it. Due to the length of the article I will divide it into three parts. This is part 3 of 3.

## The Bad

The worst thing to highlight would be its complexity. Some of you may think that there are other operating systems that are even more tedious to configure and prepare (like Arch Linux) or even more complex to understand and use (like NixOS) but that doesn't mean that Debian is not an operating system for beginners.

I will now explain in more detail what I am trying to express, to simplify it a bit, I have had two experiences with Debian:

1. My first experience which was absolute chaos.
2. My second experience, which is the current one and is where I have learned to love this operating system.

### My first experience

Debian is not an operating system for Linux novices, it gives you too much freedom, you can contaminate the operating system very easily with packages that are from other subdistributions (as happens with packages compiled for Ubuntu), and since it is not immutable, if you corrupt the system in the slightest or you do not know what you are doing at any given time (for example, using sudo or the root user all the time), you find yourself with a very complex operating system to fix the errors you have created while trying to fix the errors you had in the first place. That makes it possible to crash the operating system very very very easily. At least in Windows there is always an easy way to fix things (usually). So I would follow the following recommendations so that you do not spend entire nights without sleep, trying to fix a problem that you have caused, because you followed a guide without understanding the commands, and that guide was for Ubuntu and you have a corrupted and completely unstable system.

#### Recommendations for using Debian

1. Always know what exactly all the commands you run do. It seems obvious, but it's hard for a novice to know, and you can study the commands or ask a ChatBot like ChatGPT.
2. If you are not convinced by any guide you see on the Internet, do not follow it. Because if you do, you can easily crash your system. As we say in Spain: "The cure is worse than the disease."
3. Do not use the **root** user, put it with nologin, and use **sudo** as a substitute. This is an important security measure.
4. Learn to use the firewall to make your computer more secure. If you do not want to learn the arp tables, you can use **UFW** which is very good (the only problem it has is that you cannot configure the network layer, ping requests, etc.).
5. For your first Linux distro you should not use Debian, use an immutable distribution like VanillaOS, because if you crash the operating system (which you will end up doing) you can fix it in seconds and not in an entire night (hopefully).
6. Before switching to Debian, look for a replacement for your applications that you use on Windows and/or Mac. Because the vast majority (except for games) you will not be able to use.
7. Many of the shortcomings of Linux can be fixed by using a virtual machine with Windows. Don't feel ashamed when using Windows, you don't have to be a Linux purist.
8. If you feel overwhelmed/frustrated you can always go back to an operating system that you feel comfortable with. You can try again later. Although remember that you learn from effort.
9. All of us who use Debian know that if a problem ever occurs we can spend hours trying to fix it. That's why things are usually modified very little, like companies do with servers. 10. Official Debian updates will **never** break the operating system, so don't be afraid to update (which is true for Arch or Windows).

Most of the recommendations I've given above can be applied to Linux in general and not just Debian.
These are some of my recommendations, in the future I'll try to explain more (so as not to make this article too long).

### My second experience

When you already have an intermediate knowledge of Linux, it's very rewarding. You have a stable operating system completely configured to your liking. Unlike my first experience, I've now enjoyed it all the way, so much so that I'll use Debian from now on and won't change to another operating system.

### Updates are slow

Get used to it, unlike Windows and Arch that update practically every day, Debian usually does it 2 or 3 times a month. Normally these updates are security updates, since the Debian team doesn't have time to fully test all the programs beforehand. While that seems like a good thing to me, it is a guarantee. If I upgrade i know that the update is not going to misconfigure anything or destabilize the system.

Most of the time I update the operating system, the updates are for Flatpak applications.

### Special thanks

After all these complaints, I have to admit that Debian is my favorite operating system, I love it, but that doesn't mean I don't have problems. (Like everything in life)
My intention is not to bother or offend anyone or any community. It's just my opinion on the experiences I've had.
I also don't want to discredit the amazing work that these communities do on the infinite projects of this nature, I'm aware that it's a lot of effort and work and on top of that for free. Therefore, I want to thank all the people and groups present in these projects, since they are the ones who allow us to have this freedom (which I complain so much about). Thank you very much from the bottom of my heart.

In the future I will try to explain more experiences and adventures with Debian. 😊

With this trilogy I finish my opinion on Debian. As you may have guessed, it is my favorite operating system, I love it even with all its defects. ❤️

Regards, [emilio.red](http://emilio.red) 😎