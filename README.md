URL: [https://github.com/sophiequestion/webcoding](https://sophiequestion.github.io/webcoding/)
Source of codes: UI in Figma, with Anima plug in I downloaded the CSS+HTML and HTML codes, and it generated the site (with bugs), like there was no picture only the placeholder, checked the bugs and fix them (I got help in javascript part a bit)
Source of images
What kind of js code did you use: Emailjs for the contact form
What kind of font did you use: Borel, Roboto and Yarndings 12
Your name: Kérdy Zsófi

# Almodóvar Tribute Site

A static, responsive portfolio-style website celebrating the work of Spanish filmmaker Pedro Almodóvar. Features a hero section, bio, film gallery with lightbox and captions, a filmography table, and a contact form powered by EmailJS.

## Table of Contents

1. [Features](#features)  
2. [Demo](#demo)  
3. [Getting Started](#getting-started)  
   - [Prerequisites](#prerequisites)  
   - [Installation](#installation)  
4. [Configuration](#configuration)  
   - [EmailJS Setup](#emailjs-setup)  

## Features

- **Hero Section** with full-width background image and overlay headline  
- **About Section** summarizing Almodóvar’s career  
- **Film Showcase** gallery  
  - Clickable thumbnails open in a lightbox  
  - Keyboard (← → Esc) and click-away controls  
  - Custom captions for each film  
- **Filmography** table with CSS Grid layout  
- **Contact Form**  
  - Built with EmailJS (no backend required)  
  - Validates name, email, message, and “Terms” checkbox  

## Demo

Live demo on GitHub Pages

## Getting Started

### Prerequisites

- Modern web browser  
- (Optional) Local HTTP server (e.g. Live Server for VS Code, `python -m http.server`)

### Installation

Clone the repository and open in your browser:

```bash
git clone https://github.com/...
cd almadovar
```
then open index.html or serve with a local server

## Configuration

### EmailJS Setup

1. Sign up at [EmailJS.com] and create a Service ID, Template ID, and User ID.  
2. In `index.html`, replace the placeholder IDs in the script:

   ```js
   emailjs.init("YOUR_USER_ID");
   emailjs.sendForm("YOUR_SERVICE_ID", "YOUR_TEMPLATE_ID", this);
   ```
3. Ensure your EmailJS template fields match the form field names: name, email, message.
