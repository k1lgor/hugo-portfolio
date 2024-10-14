---
title: MAC changer
summary: A script to automatically change your MAC address
tags:
  - Bash
  - Shell
date: '2024-08-24T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: ''
  focal_point: Smart

links:
  - icon: github
    icon_pack: fab
    name: GitHub
    url: https://github.com/k1lgor/macchanger
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

## Setup

```bash
git clone https://github.com/k1lgor/macchanger.git
cd macchanger
chmod +x macchanger.sh
sudo ./macchanger.sh
```

## Info

The script works with Arch, Debian, Ubuntu, RHEL, Fedora, SuSe-based distros it will check if `ifconfig` and `macchanger` exist and install them accordingly.

## Usage

The script begins with a welcome message displayed in ASCII art. It then checks if the script is being run as root using the EUID environment variable. If it's not being run as root, it displays an error message and exits.

The script defines a function called `check_ifconfig` that checks if the `ifconfig` command is installed and installs it if necessary. It does this by checking the availability of `ifconfig` using the type command and then installing it using the appropriate package manager based on the user's operating system. The supported distributions are Arch, Debian, Fedora, RHEL, and SUSE-based distros.

The script also defines a function called `checking_distro` that determines the user's operating system by checking the contents of the `/etc/os-release` file. It supports distributions such as Arch, Debian, Fedora, RHEL, SUSE, and Ubuntu.

The `all_devices` function lists all network interfaces except 'lo' by iterating through the output of the `ifconfig` command, filtering out the 'lo' interface, and storing the remaining interfaces in an array.

The `list_all_devices` function prints the list of network interfaces except 'lo' along with their corresponding numbers.

The `change_mac` function changes the MAC address of a selected network interface. It first checks if the `macchanger` command is installed and installs it if necessary. It then brings down the selected network interface, changes its MAC address using the `macchanger` command, and brings it back up.

Finally, the script calls the necessary functions, lists all network interfaces except 'lo', and prompts the user to choose a network interface by its number. After the user selects a network interface, the script changes its MAC address using the `change_mac` function.
