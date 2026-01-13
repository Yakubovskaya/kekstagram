# Kekstagram

A web-based image sharing service built with JavaScript.  
Allows users to upload photos, apply visual effects, add descriptions, and explore images uploaded by others.

## About the Project

**Kekstagram** is a frontend application inspired by social photo platforms.  
Users can upload images, edit them in a modal editor (scaling, effects, hashtags, comments), and publish them to a remote server.  
The app also loads and displays photos from other users, providing filtering and full-screen preview functionality.

The project focuses on working with forms, validation, asynchronous requests, UI state management, and image manipulation.

## Features

- **Image upload & preview** using a custom-styled file input  
- **Image scaling** from 25% to 100% (step 25%)  
- **Built-in effects**:
  - Original (no filter)
  - Chrome (grayscale)
  - Sepia
  - Marvin (invert)
  - Phobos (blur)
  - Heat (brightness)
- **Effect intensity control** via slider powered by **noUiSlider**
- **Hashtag system** with strict validation rules (up to 5 tags)
- **Comment support** (up to 140 characters)
- **Form validation** using **Pristine** with inline error messages
- **AJAX form submission** (`multipart/form-data`) with loading state
- **Success and error notifications** with keyboard and overlay controls
- **Dynamic gallery** of user images loaded from the server
- **Full-screen image preview** with likes and comments
- **Progressive comments loading** (5 at a time)
- **Image filtering**:
  - Default order
  - Random (10 unique images)
  - Most discussed (by comment count)
- **Debounced rendering** when switching filters (500 ms)

## API

- **Load images** — [`GET /kekstagram/data`](https://25.javascript.htmlacademy.pro/kekstagram/data)
- **Upload image** — [`POST /kekstagram`](https://25.javascript.htmlacademy.pro/kekstagram)

## Tech Stack

- JavaScript (ES6+)
- HTML5 / CSS3
- **noUiSlider** — effect intensity slider
- **Pristine** — form validation
- Fetch API / AJAX

## Project Purpose

Educational project aimed at practicing:
- Form handling and validation
- Working with modals and keyboard events
- Asynchronous data loading
- DOM manipulation and templating
- Client-side filtering and performance optimization

## Deployment

[Link](https://yakubovskaya.github.io/kekstagram/)
