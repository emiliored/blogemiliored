---
title: "🔥 Welcome to my blog 🔥"
date: 2024-09-03T04:05:28+02:00
author: "emilio.red"
description: "Brief introduction and various considerations"
draft: false
---

# Hello everyone
In this blog post I will explain my ambitions and goals with this blog and the page.

# Context
I recently bought the domain [emilio.red](emilio.red) and I am looking to create an image of myself on the internet that allows me to develop my interests without having to give up my privacy and security along the way, let me explain.

## Privacy
By using the new domain I can use new email aliases that allow me to mask my real email address, which I am trying to centralize; by centralize, I mean that before I had several different email accounts that I used to "filter" the emails a bit. The problem with that is that it was chaos because I didn't know exactly which accounts were assigned to which emails (this fact is important, I will explain it in the next section).

### Account data leaks and theft
When you create an account on the Internet, you always and I mean ALWAYS have to assume that the database on the account server will be leaked and your data will practically be made public.
My experience in Backend development has taught me that although it is not a complex process (making the server follow industry security standards), practically no service on the Internet respects it because it is a tedious process.

There are numerous cases of data leaks such as:
- The numerous Lastpass leaks: [SourceExample](https://www.redeszone.net/noticias/seguridad/gestor-contrasenas-lastpass-filtracion-datos/)
- Leaks such as Twitch (which leaked not only backend code, but also financial data of streamers): [SourceExample](https://vandal.elespanol.com/noticia/r12740/la-gran-filtracion-de-twitch-esto-es-lo-que-ganan-auronplay-ibai-thegrefg-o-rubius)

And I could continue giving more examples (there are countless similar cases) but honestly I'm too lazy.

Although in the future I would love to put up a guide on how to obtain data leaks using the I2P network (there are many simpler ways, but when I learned the concepts of the I2P network I was fascinated).

### Organizing emails and accounts using email aliases
Due to the above, I found it necessary to create these email aliases. I am using Cloudflare for this, because it is convenient and cheap. I know that some people think that Cloudflare is also a sword of Damocles when it comes to privacy, but the truth is, I don't give it much importance.

In my project and my use cases I see it as useful and necessary. In this way I can filter through rules (filters in Thunderbird) of email (in Outlook) the emails that I receive through the assigned aliases, so that they go directly to Spam, temporary folders, the mailbox, etc.

In this way I keep a mask (the email alias) between the sender and me. They only discover my real email if I want them to, guaranteeing my privacy.

### Personal domains are less susceptible to bans
Let me explain:
- One day when I was in college, I used a proxy to try to bypass the Firewall, and the only reason it failed was because it couldn't resolve the domain's DNS request because I was using a free public domain on the internet, which was widely known and when I banned that domain, my subdomain was banned too.
- It took me a while to realize it, although it's a pretty silly problem, because you connect directly from your proxy's IP and voila, it works, but these kinds of things are usually obfuscated enough in the Firewalls so that you give up and leave it.
- The proxy worked perfectly and if I had used a personal domain, it wouldn't have happened to me.

In the future I will explain my adventures and how I managed to bypass the Firewall easily and in different ways at university.

## Security
### Using Hugo
Using Hugo (the static web page generator I used for you to read this article) is necessary because it allows me to:
- Maintain security on the page and on the blog, as there is nothing dynamic or any engine (such as Wordpress for example) the only information they can obtain is what I publish with Hugo (obviously the idea is that I only publish what I want to publish, therefore it is public).
- It allows me to create web pages with a certain degree of dynamism completely free. This web page is being hosted on Cloudflare for free (I only pay for the domain).
- I can create an infinite number of web pages using this technology for different areas, since its hosting and the creation of the subdomains is completely free.

### Public PGP Key
I have posted my public PGP key on the page (pgp.emilio.red), so that people who want to contact my email can encrypt the messages, in such a way that their privacy is guaranteed, as well as the security of the authentication and the security that only the reciever can read the recipient.

Feel free to send me encrypted emails to the public address [contact@emilio.red](mailto:contact@emilio.red)

### Technological Independence
This is a complex section and one I would like to expand on in the future, but basically the use of these technologies and the domain allows me to control exactly how they are used, what they do and for what purpose.
- Ensuring that the published data and its services are platform agnostic. For example, the use of email aliases allows me to choose which provider to use and change it at any time.
- The data published in Hugo can be easily adapted to other systems and/or services such as Wordpress, etc.

# Objectives
In this introduction to the blog I have talked a bit about everything, about my thoughts and reasoning for using it. This is what this page is about. I hope you like it and look forward to my next posts, as I will try to make guides on numerous technologies that I have been using and learning over the years, and I will explain in detail why I use them, and how they differ from the competition.

Regards, [emilio.red](emilio.red) 😎

