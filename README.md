Intrepid Flights - Landing Page
A high-performance, desktop-optimized landing page for Intrepid Flights, a professional aerial photography and geographical mapping service based in the Twin Cities, MN.

This repository contains the source code for the main entry point of the website, featuring rigorous SEO optimization, device-specific routing, and an accessible, dark-themed UI.

🚀 Features
📱 Intelligent Device Detection
The site utilizes a custom JavaScript implementation to manage user experience across devices:

Desktop & iPad: Renders the full cinematic split-screen experience.

Mobile (Phones/Small Screens): Automatically redirects to the mobile-optimized path (/home/) to ensure usability on smaller viewports.

Logic: Uses navigator.userAgent and window.innerWidth to differentiate between iPads (which keep the desktop view) and other mobile devices.

🎨 Design & UI
Split Layout: Fixed sidebar navigation with a scrollable hero section.

Typography: Pairs Oswald (headers/navigation) with Inter (body text) for a clean, industrial aesthetic.

Cinematic Hero: Full-viewport background imagery with CSS animations (fadeInUp) for the main headline.

Interactive Elements: Custom hover states and Haptic Feedback (Vibration API) on menu interaction.

♿ Accessibility (A11y)
ARIA Labels: Fully implemented on navigation buttons (aria-pressed) and contact links.

Focus States: High-contrast visible outlines for keyboard navigation.

Reduced Motion: CSS media queries respect user operating system preferences for reduced motion.

Contrast: Text colors adhere to high-contrast standards for readability against the dark background.

📈 SEO & Analytics
Meta Tags: Extensive Open Graph (Facebook/LinkedIn) and Twitter Card integration.

Schema.org: JSON-LD structured data for ProfessionalService including geo-coordinates and pricing.

Microsoft Clarity: Integrated heatmap and user behavior tracking.

🛠️ Technologies Used
HTML5: Semantic markup.

CSS3: Flexbox, CSS Variables, Keyframe Animations, Media Queries.

JavaScript (ES6): Device detection logic and UI interaction handling.

External Assets:

Font Awesome (Icons)

Google Fonts (Inter & Oswald)

📂 Project Structure
Plaintext

/
├── index.html          # Main entry point (Desktop view)
├── /home/              # Mobile redirect destination (External)
├── indigo.png          # Favicon
├── image.jpeg          # Main Hero Background
└── README.md           # Project Documentation
🔧 Usage
Clone the repository:

Bash

git clone https://github.com/yourusername/intrepid-flights.git
Open locally: Simply open index.html in your preferred web browser.

Note: To test the mobile redirect locally, use your browser's DevTools to simulate a mobile device (e.g., iPhone SE).

👤 Author
Joshua Stafki

Website: intrepidflights.com

Location: Hanover, MN

📄 License
© 2025 Intrepid Flights. All Rights Reserved.
