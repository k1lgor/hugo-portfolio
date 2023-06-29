---
title: MAC changer
summary: A script to automatically change your MAC address
tags:
  - Bash
  - Shell
date: '2022-05-01T00:00:00Z'

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

To get started with `macchanger`, follow the steps below:

1. Clone the repository to your local machine:

```bash
git clone https://github.com/k1lgor/macchanger.git
```

2. Change into `macchanger` directory:

```bash
cd macchanger
```

3. Make the script executable:

```bash
chmod +x macchanger.sh
```

4. Execute the script with sudo:

```bash
sudo ./macchanger.sh
```

This will run the macchanger script with administrative privileges.

## Compatability

The macchanger script is compatible with the following Linux distributions:

- Arch Linux
- Debian-based distributions (e.g., Ubuntu)
- Red Hat Enterprise Linux (RHEL)
- Fedora
- openSUSE-based distributions

## Dependencies

The script checks for the presence of `ifconfig` and `macchanger` commands and installs them if they are not already available on your system. These dependencies are necessary for macchanger to function properly.
