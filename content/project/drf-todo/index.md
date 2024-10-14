---
title: Django To-Do App
summary: This is a simple Todo application built with Django
tags:
  - Python
  - Web
date: '2024-02-09T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: ''
  focal_point: Smart

links:
  - icon: github
    icon_pack: fab
    name: GitHub
    url: https://github.com/k1lgor/drf-todo
  - icon: python
    icon_pack: fab
    name: Python
  - name: Django
  - name: Docker
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

This is a simple Todo application built with Django. It allows users to create, update, and delete their todos.

## Features

- User Authentication: Users can sign up, log in, and log out.
- Todo Management: Users can create new todos, mark them as completed, or delete them.
- Todo Details: Each todo has a title, optional memo, creation date, and an optional completion date.
- Importance: Users can mark todos as important.

## URLs

- `/signup/`: Sign up for a new account.
- `/login/`: Log in to your account.
- `/logout/`: Log out of your account.
- `/`: Home page, showing all current todos.
- `/create/`: Create a new todo.
- `/current/`: View all current todos.
- `/completed/`: View all completed todos.
- `/todo/<int:todo_pk>`: View details of a specific todo.
- `/todo/<int:todo_pk>/complete`: Mark a specific todo as completed.
- `/todo/<int:todo_pk>/delete`: Delete a specific todo.

## Models

### User

This model represents the users of the application. It includes fields like username, password, and email.

### Todo

This model represents the todos. It includes fields like:

- `title`: The title of the todo.
- `memo`: An optional memo for the todo.
- `created`: The date when the todo was created.
- `datecompleted`: An optional date when the todo was completed.
- `important`: A boolean field to mark the todo as important.
- `user`: A foreign key to the User model, representing the user who created the todo.

## Docker

This project uses Docker for easy setup and deployment. The `Dockerfile` in the root directory of this repository defines the Docker image for this project.

### Dockerfile

The `Dockerfile` specifies the base Python image from Docker Hub. It then copies the project files into the Docker image and installs the necessary dependencies using pip.

Here's a brief overview of the commands in the `Dockerfile`:

- `FROM python:3.11-alpine`: This line specifies the base image. In this case, it's the official Docker image for Python 3.11 running on Alpine Linux.
- `WORKDIR /app`: This line sets the working directory in the Docker image to `/app`.
- `COPY . /app`: This line copies the project files into the Docker image.
- `RUN pip install -r requirements.txt --no-cache-dir`: This line installs the necessary Python dependencies specified in the `requirements.txt` file.

### Building the Docker Image

To build the Docker image, navigate to the root directory of the project and run the following command:

```bash
docker build -t todo-app .
```

This command builds a Docker image and tags it as `todo-app`.

### Running the Docker Image

To run the Docker image, use the following command:

```bash
docker run -p 8000:8000 todo-app
```

This command runs the Docker image and maps port 8000 in the Docker container to port 8000 on your machine. The application will then be accessible at `http://localhost:8000`.
