---
title: BMI Calculator CLI
summary: This is a command-line interface (CLI) tool for calculating body mass index (BMI) based on user input for weight and height.
tags:
  - Go
date: '2023-04-18T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: ''
  focal_point: Smart

links:
  - icon: github
    icon_pack: fab
    name: GitHub
    url: https://github.com/k1lgor/bmi
  - icon: golang
    icon_pack: fab
    name: Golang
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

This is a command-line interface (CLI) tool for calculating body mass index (BMI) based on user input for weight and
height.

## Features

- Calculate BMI based on weight (in kilograms) and height (in centimeters).
- Display the calculated BMI value and corresponding weight category (underweight, normal, overweight, or obese).
- Allow for input of weight and height either through command-line arguments.
- Validate user input to ensure that weight and height are valid numeric values.

## Usage

To calculate your BMI using this CLI tool, run the following command:

```go
bmi <weight> <height>
```

Replace <weight-in-kg> with your weight in kilograms (e.g., 70) and <height-in-m> with your height in meters (e.g.,
175).

## Installation

To install the BMI Calculator CLI tool, simply download the executable file for your operating system from the releases
page on GitHub.

Alternatively, you can clone the repository and build the executable file yourself using Go:

```go
git clone git@github.com:k1lgor/bmi.git
cd bmi
go build
sudo mv bmi /usr/bin
```

## License

This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.
