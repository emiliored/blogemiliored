---
title: "Debian The Ugly"
date: 2024-09-05T22:20:06+02:00
author: "emilio.red"
description: "My opinion on using Debian and its features."
draft: false
---

Hi everyone, today I'm going to share my thoughts and opinions on the Debian operating system.

# Debian

Debian is a GNU/Linux operating system that stands out for its incredible stability, security, and performance. So much so that many Linux distributions are based on it. Due to the length of the article I'm going to divide it into three parts. This is part 2 of 3.

## The Ugly

In this article I'm going to explain the tedious parts about my experience with Debian.

### The Setup

It's a pain, that's all. Ok, let me explain. The thing about Debian is that it gives you absolute freedom, that's a good thing, but if you come from other operating systems, you'll be used to everything being neatly laid out, interconnected, and you having to do practically nothing, as is the case with Windows or systems like Ubuntu. That doesn't happen in Debian, the default configuration is not worth much, you'll have to spend hours and even days configuring everything exactly as you want, and in the end, everything has its ugly side.

It gives you a lot of freedom, but you have to spend a lot of time configuring everything and in the end you are responsible for everything. As I already said, if you make a bad configuration you know it's your fault, there are no other external factors. Therefore, you have to spend a lot of time thinking about how to do things and how you want them to be, for example:

- You can implement a new configuration that breaks your operating system and you get a Kernel Panic.

You can think, well, it was due to the user's negligence, so what. But the problem is that because the default configuration is pretty useless, you have to go through a lot of configuration problems just to get ahead and have an operating system that you don't have the courage to use. That kind of "responsibility" or tedium, you don't have in other operating systems.

### Linux is decentralized in nature

Let me explain, if you have a problem with Windows, you search for it on Google and follow the steps on pages that bombard you with ads. At least, you know that those steps can probably help you, because in Linux, I assure you that they don't have to.

In Linux, there are many distributions, many package managers, many different configurations, many different desktop environments, etc. That can be a good thing, because in the end you have the freedom to make your Linux the way you want it, the problem is that most of the time you won't fully understand everything. That means, you can understand that you have a video driver installed, and you have a certain desktop environment, but the error can be in the backend of the desktop environment that has not been correctly adapted to that driver (as happens with Wayland and Nvidia drivers) and in the end, you can't blame anyone.
- The community has ported a driver by reverse engineering it from Nvidia,
- the community has created and maintained a multipurpose desktop backend (X11) for almost 30 years,
- the community has created and maintained a desktop frontend so you can use your operating system normally (for example KDE),
- and the developers of your Linux distribution have put it all together for you (In this case the Debian team).

After all that titanic work that has been done by several different communities, sometimes even from different Linux distributions (it may be for example that it is not officially supported by your distribution, but you can use those technologies), the only responsibility for everything falls on you, nothing and nobody guarantees that it will work, or that when you put it all together it will work. It may sound fatalistic, but this is the theory in reality, and it is what Linux communities usually do not tell you.

In practice, the developments and projects in Linux, created by different communities are usually very very very good and professional. Normally everything interconnects correctly and you usually don't have any problems. The problem is when this isn't the case (for example with proprietary drivers).

#### Nvidia Experience

If you have an older Nvidia graphics card (before the RTX 20xx series, because Nvidia made the drivers open source), sooner or later you're going to have to install Nvidia's proprietary drivers. You will only stick with Nouveau drivers (the reverse engineering project that ported Nvidia drivers to Linux making them open source) if you are willing to waste half of your graphics card's capability, because half of the features are not implemented at the software level (at the API level), for example:
- With the Nouveau driver you cannot have the 3D graphics library therefore,
- With the Nouveau driver you cannot play games on Linux (only 2D games)

And if you have special features of your graphics card, such as for example, making use of the Nvidia CUDA calculation library to take advantage of your graphics card beyond video games (for example you may need to calculate hashes or use it for AI) if you have the Nouveau drivers forget about it.

Then you need to install the proprietary drivers if you want to take advantage of your graphics card. The biggest problem with this is that Nvidia doesn't give a shit about having those drivers updated and well programmed, that is, they provide the ABI and the API that developers of other projects can use to communicate with the graphics card, because as it usually happens with this type of proprietary projects, they don't care, they update the drivers whenever they want, if you have a bug they may never fix it, etc. In other words, Nvidia only prioritizes Windows drivers, and Linux drivers for what. At least it has always been like this with Nvidia (it's not something new) although with the new graphics cards I have no idea (I suppose that since it is open source this should not happen anymore). Due to the decentralized nature of Linux projects, the only guarantee you have that things will work correctly is that they are open source, because Nvidia will never adapt anything beyond their drivers.

Therefore we come to the conclusion that I mentioned in previous sections and that is that it is always better that everything is open source, because you cannot trust any company to properly maintain the projects.

In Debian it has always been said that installing drivers is a matter of trying and testing, if you are lucky it works, if not try another way. If you have several Kernel Panics along the way it is your problem, it is your responsibility to fix it, since in the end **you have to do everything on your own**.

### There are some problems that you will never be able to solve

This section has a good and an ugly thing. Let me explain:

Because drivers ported to Linux are usually adaptations of Windows (usually open source) their behavior is different. According to the intellectual property law or Copyright, anyone can adapt and make their own version of any software (whether proprietary or not) as long as it varies in the code, that is, it is an adaptation and is not identical.

Well, in Linux these driver adaptations sometimes make them behave differently than in Windows. That is, with the same hardware, the software and the user experience is different, because the firmware or drivers (which are the libraries used to communicate the software and the hardware) is an adaptation and is therefore different in Linux than in Windows.

You might think, well, what does it matter. The fact is that this means new problems (bugs) or that the experience is slightly different.

For example:
- My audio driver does not normalize the audio so the user experience is different. I notice that sometimes I do not hear the low sounds and I hear the high sounds very loud. This did not happen in Windows, because the driver or some library did the sound normalization. So, with the same hardware, the user experience is different because of that adaptation.
- Another example is proprietary codecs, in Linux they are not installed by default, so sometimes you find that suddenly your experience on a web page is ruined because the browser needs that proprietary codec to display the content (it could use another equivalent codec from your system, but many times it doesn't happen) and the page crashes.
- My computer has two graphics cards, one integrated from Intel and one dedicated from Nvidia. When I used Windows I had a rather annoying bug that happened when I used the integrated one, the computer didn't use the memory of the dedicated one (VRam) and used the computer's RAM, so there were stutters when playing the content. Well, that doesn't happen to me in Linux (Debian specifically), I don't have that error in Linux, that's great of course, but it helps me explain the following problem.

**As drivers are proprietary software adaptations and do not behave the same, new bugs may arise or bugs present in other systems may be fixed (because they have been patched in that version or did not exist in the first place) and you have slightly different experiences** you have to be able to adapt and not get frustrated.

### Special thanks

After all these complaints, I have to admit that Debian is my favorite operating system, I love it, but that does not mean that I do not have problems. (As with everything in life)
My intention is not to bother or offend anyone or any community. It is only my opinion on the experiences I have had.
I also do not want to discredit the amazing work that these communities do on the infinite projects of this nature, I am aware that it is a lot of effort and work and on top of that for free. Therefore, I want to thank all the people and groups present in these projects, since they are the ones who allow us to have this freedom (which I complain so much about). Thank you very much from the bottom of my heart.

I will continue with the explanation in part 3:Debian The Bad.

Greetings, [emilio.red](http://emilio.red) 😎