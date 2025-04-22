# Intrepid Flights - Drone Photography Website Template

**Version:** 1.0
**Date:** 2025-04-22
**Project:** Single-page website for a drone photography/videography service.

## Description

This repository contains the HTML, CSS, and JavaScript code for a modern, creative, and responsive single-page website template designed for **Intrepid Flights**, a drone photography and videography service potentially based in **Ramsey, Minnesota**. It features an immersive hero section, dynamic content display, smooth animations, and a professional look tailored to showcase stunning aerial visuals.

The design emphasizes visual impact and user engagement, aiming for an innovative feel suitable for a tech-forward photography business.

## Features

* **Immersive Hero Section:** Full viewport height section with a video background (recommended) or image fallback, featuring a text overlay and a clear call-to-action.
* **Sticky Header:** Navigation bar stays fixed at the top, changing background color on scroll for better visibility.
* **Responsive Design:** Adapts gracefully to various screen sizes (desktops, tablets, mobiles) using Flexbox, Grid, and Media Queries.
* **Mobile-Friendly Navigation:** Includes a toggleable hamburger menu for smaller devices.
* **Smooth Scroll & Animations:**
    * CSS-driven smooth scrolling for anchor links (`#about`, `#services`, etc.).
    * Sections fade and slide in subtly as the user scrolls down, powered by the `IntersectionObserver` API.
    * Hover effects on navigation links, buttons, service items, and gallery images enhance interactivity.
* **Dynamic Gallery:** A grid layout for showcasing portfolio images with interactive hover overlays displaying titles and descriptions.
* **Animated Service Icons:** Service items include icons with subtle animations on hover.
* **Contact Form:** A clean, styled contact form section (requires backend integration).
* **Customizable:** Easily change the color scheme and fonts using CSS variables.
* **SEO Friendly:** Basic meta tags included (description).
* **Dynamic Copyright Year:** Footer automatically displays the current year.

## Technology Stack

* **HTML5:** Semantic structure for content.
* **CSS3:**
    * Styling, layout, and animations.
    * **CSS Variables:** For easy theme customization (colors, fonts).
    * **Flexbox & CSS Grid:** For responsive layouts.
    * **Transitions & Animations:** For hover effects and scroll-triggered effects.
    * **Media Queries:** For responsiveness across devices.
* **JavaScript (Vanilla ES6+):**
    * DOM manipulation for dynamic behaviors (sticky header, mobile menu).
    * **Intersection Observer API:** For efficient scroll-based animations.
    * Dynamic content updates (e.g., footer year).

## Setup & Usage

1.  **Save the Code:** Save the complete HTML code block (including `<style>` and `<script>` tags) as an `index.html` file.
2.  **Replace Placeholders:** This is crucial! Go through the `index.html` file and replace all placeholder content with your actual assets and information:
    * **Hero Video:** Replace `"placeholder-drone-video.mp4"` in the `<video>` tag with the path to your actual video file. Ensure the video is web-optimized (consider format like MP4/WebM and reasonable file size).
    * **Hero Fallback Image:** If using the image background option or as a fallback, replace `'placeholder-hero-image.jpg'` with your image path.
    * **About Image:** Replace the `src` in the `<img>` tag within the `#about` section.
    * **Gallery Images:** Replace all `https://via.placeholder.com/...` URLs in the `#gallery` section with paths to your actual portfolio images. Update the `alt` text and the overlay `<h4>` and `<p>` content for each image.
    * **Service Icons:** The current icons (📸, 🎬, etc.) are text emojis. For a more professional look, consider integrating an icon library (like Font Awesome) and replacing these emojis with appropriate icon classes.
    * **Text Content:** Update all descriptive text (headings, paragraphs in About, Services, Contact sections) to accurately reflect Intrepid Flights' specific offerings, mission, and story.
    * **Location:** Update the location mentioned in the About section and Footer (currently mentions "Ramsey, MN" based on context).
    * **Contact Form Action:** Change the `action="submit-form.php"` attribute in the `<form>` tag to the URL of your actual backend script that will process the form data.
    * **Social Media Links:** Replace the `#` in the `href` attributes of the footer social links (`<a>` tags) with your actual social media profile URLs. Update the `data-icon` attributes if you implement real icons.
3.  **Backend for Contact Form:** The contact form requires a server-side script (e.g., PHP, Node.js, Python backend, or a third-party service like Formspree) to receive and process the submitted data (like sending it to an email address). The provided HTML only includes the front-end structure.
4.  **Web Hosting:** Upload the `index.html` file and all your assets (images, video) to a web hosting provider to make the website live.

## Customization

* **Colors & Fonts:** Easily change the website's look and feel by modifying the CSS variables defined within the `<style>` block under the `:root` selector.
    ```css
    :root {
        --primary-color: #0a192f; /* Deep Navy */
        --secondary-color: #1e3a5f; /* Slightly Lighter Navy */
        --accent-color: #ff6b00; /* Bold Orange */
        --text-light: #ccd6f6; /* Light Grey/Blue */
        /* ... other variables ... */
        --font-primary: 'Poppins', sans-serif;
        --font-monospace: 'Roboto Mono', monospace;
    }
    ```
* **Adding/Removing Sections:** You can add new `<section>` blocks or remove existing ones. Remember to update the navigation links in the `<header>` if you make changes.
* **Gallery/Service Items:** Add or remove `<div>` blocks within the `.gallery-grid` or `.services-grid` to modify the number of items displayed.

## File Structure (Recommended if separating files)

While the provided code has CSS and JS embedded in the HTML for simplicity, a typical project structure would be:
