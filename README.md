# Intrepid Flights - Web Portal

A desktop-optimized, static landing page for **Intrepid Flights**, providing professional aerial photography, real estate drone services, and geographical mapping in the Twin Cities and surrounding communities. 

The site features a modern, high-contrast dark theme, ADA-compliant accessibility, and built-in mobile redirection.

## 🚀 Features

* **Device-Aware Routing:** Includes a JavaScript device-detection script that automatically redirects mobile and small-screen users (excluding iPads) to the mobile-optimized `/home/` directory.
* **Accessible Design (ADA Compliant):**
  * Visible focus states for keyboard navigation.
  * ARIA attributes (`aria-pressed`, `aria-label`, `aria-hidden`) for screen readers.
  * Reduced motion media queries (`prefers-reduced-motion`) to disable animations for users with vestibular disorders.
* **SEO & Social Graph Optimization:**
  * Semantic HTML5 and comprehensive meta tags.
  * OpenGraph (OG) and Twitter Card integration for rich social media sharing.
  * Embedded JSON-LD schema (`ProfessionalService`) for enhanced search engine visibility, including local business coordinates and contact details.
* **Analytics Integration:** Built-in tracking via Microsoft Clarity.
* **Responsive Interactive UI:** A fixed-layout sidebar with smooth CSS transitions and JavaScript-toggled active states for the services menu.

## 🛠 Tech Stack

* **Markup:** HTML5
* **Styling:** CSS3 (Custom Properties/Variables, Flexbox, Keyframe Animations)
* **Scripting:** Vanilla JavaScript
* **Typography:** Google Fonts (Inter & Oswald)
* **Icons:** FontAwesome 6.5.0

## 📂 Architecture Overview

The single-page application is split into a strict two-column desktop layout:

1. **Sidebar (`#menu-panel`):** Houses the brand identity, location details, interactive services menu, contact information (telephone, email), social media links, and footer navigation.
2. **Hero View (`.hero-view`):** A large, screen-filling background image (Cancun, Mexico) with absolute-positioned geographical coordinates, a dynamic typography overlay, and a link to image metadata.

## 💻 Local Development

Since this is a static webpage with no build steps or dependencies required, deployment and testing are straightforward.

1. Clone the repository to your local machine.
2. Open `index.html` directly in any modern web browser.
3. *Note:* To test the desktop layout on a smaller screen, temporarily comment out the mobile redirect script in the `<head>` section to prevent being routed to `/home/`.
