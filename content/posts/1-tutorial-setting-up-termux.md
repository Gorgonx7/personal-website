+++
date = '2026-02-08T22:53:20Z'
draft = true
title = 'Creating a basic code environment on tablet'
tags = ['tutorial', 'termux', 'mobile', 'development']
+++

So I like writing blogs. 

I do it a lot in my day job but I very rarely get the time to write blogs outside of that. I like writing my blogs in my code editor, I'm a neovim user (obligatory I use neovim actually), which is terminal based so I throughout why not see if I can get it running on tablet.

I want to make this editor work as close to my work laptop as possible. You may ask, why not use a laptop? Good question, I had a mac I bought from work but the battery exploded and dispite my best efforts it refuses to remain with us. I also have a gaming laptop, but it gets warm for literally no reason, causing the fans to try and turn it into a helicopter. I already own a samsung tablet so I wondered if I could use that instead.

Another reason, I'm cheap, I like to own the tools I use (or at least not have to pay for them) and neovim is free and easy for me to use. Apps for writing blogs often have features locked behind a pay wall or try to push their crappy AI features that bloat the interfaces and install size. That's ignoring the other option of just buying another laptop, but really, have you seen ram prices? At time of writing 16 gig of DDR4 ram costs almost £200 because Altman et al. seem to be using silicon wafers as frisbies.

Speaking of crappy AI, I started off trying to figure out a way to get some form of terminal on tablet, and I did what I usually do, asked ChatGPT. I know, it's bad for the environment and isn't really that great at nishe things like this, but I already have limited time to figure this out and AI is good at aggrigating lots of information blatently lifted from websites on the internet. It spat out a few options, using a cloud based editor, ssh-ing into a real machine, downloading a coding app, and finally using termux.

### Why Termux? 
Termux is great because:

- It's open source (yay no pay wall)
- It's fairly popular and well documented
- I saw several reddit posts with my exact use case, nvim and a cheeky bit of golang on the side

All these reasons make it a great option for lightweight coding on the go.

### What can't it do?
It has some limitations:

- Termux isn't magic, if you don't want to root your device it has some limits, no sudo for example is a big blocker for a lot of things, but I'm a bit of an expert when it comes to that as my work doesn't let me have sudo, so I've picked up a few tricks.
- Obviously any desktop apps/desktop GUI sdks or graphics programming doesn't work, no game engine dev on tablets for me
- Some LSPs aren't currently built for android
- Mason doesn't auto install some LSPs out of the box, you'll need to manually configure some

So it's great for lightweight cli apps, and web dev as it can run apps directly on your tablet to localhost. In fact I wrote, built and previewed this blog on my tablet.


