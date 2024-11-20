# **What is this?**

This is my first github project. I want to share a .pdf file with documentation on how to install -arr apps on a Synology NAS device with (or without) a VPN. It had mainly focus on BitTorrent, but when I learned about usenet and migrated my whole srtup to useNet i updated the docs to include UseNet aswell.
Under you can read just a little snippet of my document. It spans well over 100 pages, and goes into detail on how to get the best possible experience with this setup.
It also includes a TL;DR for the lazy ones, but just for how to install it. The configs you will have to read through, since it's so much important information there.
The TL;DR also assumes you actually know a little bit about the subject, as if you do not you should read the full length docs.
Please comment anything that would make it better. Things I should add, remove, change or other things. If you get stuck anywhere, you can always drop a comment with your problem I will try to get back to you.
You can either comment here on github, or reach out to me on Reddit: https://www.reddit.com/user/MattiTheGamer/. You can also DM me on Discord @matti1003.

## Support me
I hate to ask for money, and I only really do this for fun and to help you guys out. But a guy recently commented on a reddit post of mine that I should  setup donations so I might be able to get a little kickback on my hard work. Well, I figured why not. I will not beg for your money, and don't want you to feel obligated to give me anything at all. But if you really want to support me, you can follow this link and give a custom amount of money via Paypal: https://www.paypal.com/donate/?hosted_button_id=DK7VP9RD2LEQ2

## Note
If you find any spelling mistakes, incorrect facts or anything I can improve in any way please let me know. I want to make this the best I can and hope this can one day be a "definitive" guide for *arr apps on Synology.


# HOW TO INSTALL A FULL ARR-STACK ON SYNOLOGY NAS RUNNING DSM 7.2

## Before we begin

### Info about TL;DR
Read the docs for TL;DR

### Legal Disclaimer
For legal reasons I must state that I do not condone illegal pirating of copyrighted material. 
This is made for educational purposes only. I expect that everyone who follows this guide will only use this for legal purposes.
Please never ever use this to illegally download copyrighted material such as, but not limited to, movies and TV Shows.

### Introduction
Before we start let’s figure out your needs. Do you want to download movies, tv shows, music, e-books, comics or adult videos? 
Most likely you want a combination of a lot of them. 
We also need to figure out whether you want it to be connected to a VPN. 
Here is a break-down of all the apps and their use-cases:

## What are the *arrs?

### From the wiki itself:
“Lidarr, Prowlarr, Radarr, Readarr, Sonarr, and Whisparr are collectively referred to as "*arr" or "*arrs". They are designed to automatically grab, sort, organize, and monitor your Music, Movie, E-Book, or TV Show collections for Lidarr, Radarr, Readarr, Sonarr, and Whisparr; and to manage your indexers and keep them in sync with the aforementioned apps for Prowlarr.”

### In simple terms:

Prowlarr: 
An index manager. This just means it searches for files to download on websites you assign it.

Radarr: 
When Prowlarr find a movie file, it gives it to Radarr. Radarr then send it over to a download client, like QBitTorrent. After it’s done downloading, Radarr takes it away from QBItTorrent again and rename the file appropriately before it puts it inside your Media library.

Sonarr: 
Same as Radarr, but for TV shows.

Lidarr: 
Same as Radarr, but for music

Readarr: 
Same as Radarr, but for e-books

Whisparr: 
Same as Radarr, but for adult videos

Bazarr: 
Connects with Radarr and Sonarr to download subtitles for your movies and TV shows.

Flaresolverr: 
Bypasses cloudfare solver

Overseerr:
 A requesting application where you browse or search for movies and TV shows, kinda like Netflix, and with a  click of a button they start downloading to your own media collection!

Requestrr: 
Goes together with Overseerr or Radarr and Sonarr to allow for requesting through discord chat.

Arr-stack:
The arr-stack just refers to a collection of these applications bundled and working together. 


### The apps i will cover in this guide:

I would like to cover as many as possible, but I have not used or tried some of them myself. I host on Plex, so I use Overseer, and have not tried neither Jellyseer or Ombi. Even though I’m pretty sure Jellyseer is the exact same just for Jellyfin. But you should always read the official docs yourself. Anyway, the apps I will go over is:

•	GlueTUN
•	Prowlarr
•	Flaresolverr
•	Sonarr
•	Radarr
•	Lidarr
•	Overseer
•	Requestrr
•	qBitTorrent
•	tautulli
•	Sabnzbd
•	NZBHydra2

### Hardware specs:
Read the docs for my recommendations


# Download or read through the pdf file for the full docs.

https://github.com/MathiasFurenes/synology-arr-guide/blob/main/arr-stack-rev2.0.pdf
