---
title: IMDb Web Scraper
summary: Scraper for 6 categories from IMDb
tags:
  - Python
date: '2022-10-13T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: ''
  focal_point: Smart

links:
  - icon: github
    icon_pack: fab
    name: GitHub
    url: https://github.com/k1lgor/IMDb-analysis
  - icon: python
    icon_pack: fab
    name: Python
  - name: Jupyter Notebook
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

This repository contains a Python script for scraping data from IMDb charts. The script allows you to retrieve information from various IMDb charts, including:

- Top 250 Movies
- Most Popular Movies
- Top 250 TV Shows
- Most Popular TV Shows
- Lowest Rated Movies
- Top Rated English Movies

## Info

The script extracts the title, year, and IMDb rating for each entry in the specified chart. It then writes the information to a '.csv' file in the current directory.

Please note that the script skips any Movies/TV shows that do not have a rating in the charts.

## Setup

To set up the IMDb web scraping script, follow these steps:

1. Initialize a Python virtual environment:

```bash
python -m venv venv
```

2. Activate the virtual environment:

```bash
# Windows:
.\venv\Scripts\activate
# Linux:
source venv/bin/activate
```

3. Update the pip package manager:

```bash
# Windows:
python -m pip install --upgrade pip
# Linux:
pip install pip -U
```

4. Install the required pip packages:

```bash
pip install -r requirements.txt
```

5. Usage:

```bash
python3 main.py
# or
py main.py
```
