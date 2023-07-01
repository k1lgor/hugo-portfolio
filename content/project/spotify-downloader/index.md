---
title: Spotify Downloader GUI
summary: Simple GUI for downloading your favorite playlists from Spotify.
tags:
  - Python
  - Flet
date: '2023-01-04T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: ''
  focal_point: Smart

links:
  - icon: github
    icon_pack: fab
    name: GitHub
    url: https://github.com/k1lgor/spotify-downloader-gui
  - icon: python
    icon_pack: fab
    name: Python
  - name: Flet
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ''
---

This is a simple graphical user interface (GUI) for the Spotify Downloader, written in Python using the Flet framework. The Spotify Downloader allows you to download Spotify playlists as audio files, and this GUI simplifies the process for Linux users.

## Prerequisites

Before using the Spotify Downloader GUI, make sure you have installed spotdl. You can install it by running the following command:

```bash
pip install spotdl
```

or click the button from GUI.

Please note that this GUI has been tested on Linux operating systems only.

## Usage

1. Choose Folder: Click the "Choose Folder" button to select the destination folder where the downloaded audio files will be saved.

2. Choose Bitrate: Select the desired bitrate from the dropdown menu. You can choose from various audio quality options.

3. Paste Playlist URL: Copy the playlist URL from Spotify and paste it into the "Playlist URL" input box.

4. Download: Once you have set the folder and chosen the bitrate, click the "Download" button to start the downloading process.
