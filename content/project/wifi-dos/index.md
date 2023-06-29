---
title: WiFi DoS
summary: A simple WiFi DoS script
tags:
  - Bash
  - Shell
date: '2022-03-07T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: ''
  focal_point: Smart

links:
  - icon: github
    icon_pack: fab
    name: GitHub
    url: https://github.com/k1lgor/wifi-dos
  - icon: terminal
    icon_pack: fas
    name: Bash
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

## Simple WiFi DoS Attack

This repository provides a simple script for conducting a Denial-of-Service (DoS) attack on WiFi networks. The attack utilizes the following tools:

- nmcli - Network Manager Command Line Interface
- macchanger - a utility that simplifies the manipulation of MAC addresses of network interfaces
- aircrack-ng - a comprehensive suite of tools for assessing WiFi network security

## Usage

Follow the steps below to execute the DoS attack:

1. Change the permission of the script file to make it executable:

```bash
chmod +x wifi-dos.sh
```

2. Use the following command to view all the networkds within the range of your WiFi adapter:

```bash
nmcli dev wifi
```

3. Copy the target SSID and the corresponding channel number, and replace the values in the script.
4. Execute the script with sudo, as aircrack-ng requires administrative privileges:

```bash
sudo ./wifi-dos.sh
```

## Demo

![Demo](./featured.gif)

## Disclaimer

This script is intended for educational purpose only.
The author is not responsible for any malicious use of the content.
