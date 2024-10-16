# **What is this?**

This is my first github project. I want to share a .pdf file with documentation on how to install -arr apps on a Synology NAS device with a VPN.
Under you can read just a little snippet of my document. It spans well over 100 pages, and goes into detail on how to get the best possible experience with this setup.
It also includes a TL;DR for the lazy ones, but just for how to install it. The configs you will have to read through, since it's so much important information there.
The TL;DR also assumes you actually know a little bit about the subject, as if you do not you should read the full length docs.
Please comment anything that would make it better. Things I should add, remove, change or other things. If you get stuck anywhere, you can always drop a comment with your problem I will try to get back to you.

## Note
If you find any spelling mistakes, incorrect facts or anything I can improve in any way please let me know. I want to make this the best I can an d hope this can one day be a "definitive" guide for *arr apps on Synology.


# HOW TO INSTALL A FULL ARR-STACK ON SYNOLOGY NAS RUNNING DSM 7.2

## Before we begin

### Info about TL;DR
TL;DR is at the bottom of the docs.

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

### All the different *arr apps

All the different *arr apps
Prowlarr – Index manager. It searches the torrent sites for downloads (Recommended for everyone)
Flaresolverr – Some indexers require you to solve a Cloudflare captcha. Flaresolverr can do this.
Jackett – Alternative to Prowlarr. Most find Prowlarr to be both easier to set up and better to use.
Sonarr – TV Shows/Anime Shows downloader.
Radarr – Movie downloader.
Lidarr – Music downloader.
Readarr – E-book downloader
Mylar – Comics downloader.
Bazarr – Subtitle downloader for your Movies and TV Shows.
Lazy Librarian – A program to follow authors and grab metadata for digital reading.
Whisparr – Adult videos downloader.
GlueTUN – Required for use of VPN
Plex – A frontend to your media server. It’s where you access all your media, in the style of something like Netflix. It also has a very good Spotify-like app called plexamp.
Jellyfin – Also a frontend to your media server. Jellyfin is, in contrast to Plex, open-source. This means that all of it’s features is and always will be free, but it also means that it doesn’t have the same funding and therefore might not have all of the features Plex has.
Overseerr – Allows for easy requesting of movies and TV shows to add to Plex.
Jellyseerr – Same as Overseer but for Jellyfin.
Ombi – App to request Movies and TV Shows for plex or Emby.
Requestrr – Allows for requests for Sonarr and Radarr via chat, like Discord. It can also be integrated with Ombi and Overseer.
qBitTorrent – Torrent download client.
NZBGet – NZB download client.
There are even more, but I have not gotten into these myself. These are the ones I have atleast some knowledge about.

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

### Hardware specs:
Read the docs for my recommendations


# Download or read through the pdf file for the full docs.

https://github.com/MathiasFurenes/synology-arr-guide/blob/main/arr-stack-rev1.2.pdf
