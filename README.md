**Figma Design:** (https://www.figma.com/design/jrlUWJdbxTc2bKd5dpRa5r/10X-markup-exam-project---Spotify?node-id=298-16461&t=7WcpyIlTNhAY3o8r-0)

# Dixit-Spotify Clone Project

## 📌 Project Overview

This project is a functional Spotify clone designed with a modular architecture and a focus on fluid responsiveness. The development process utilizes HTML5, CSS3, and SASS for a professional and scalable frontend structure, while Git and GitHub are used for version control and team collaboration.

---

## 🛠 Project Architecture & Setup

The project structure and core styles were established with the following technical features:

- **HTML Skeleton:** A complete semantic structure including Header, Main, and Footer sections.
- **Modular SASS & CSS:** Dedicated SASS files for each section, compiled into optimized CSS to ensure clean and maintainable code.
- **Version Control:** Implementation of Git for tracking changes and GitHub for repository management and team synchronization.
- **Global Variables:** Use of core SCSS variables and reusable mixins for design consistency.
- **Fluid Typography:** Responsive font sizes implemented via the `clamp()` function for an optimal experience across all devices (from 320px to 1440px).

---

## 👥 Team Responsibilities

The project tasks have been distributed among the team members to ensure efficient development:

| Team Member     | Assigned Modules & Sections                                  |
| :-------------- | :----------------------------------------------------------- |
| **Nora (Lead)** | Navigation (Header & Footer), Library, and Discover sections |
| **Lana**        | Home and Search sections                                     |
| **Shalva**      | Profile and Playlist sections                                |

---

## 🚀 Technical Goals

- **Mobile-First Design:** Ensuring the UI is perfected for mobile before scaling to desktop.
- **Version Control Workflow:** Using Git branches and pull requests for organized collaboration.
- **Scalability:** Leveraging SASS partials and variables for easy global updates.
- **Interactivity:** Smooth transitions and animations for a native app-like feel.

## 🚀 LatestUpdates (March 6, 2026)

**By Nora**
Implemented a fully responsive mobile-only footer navigation using a semantic <figure> and <figcaption> structure. The system features a pure CSS tab-switching logic (no JavaScript) using radio buttons and :checked selectors, enhanced with smooth fadeIn animations. Visuals are managed through SCSS variables for gradients and interactive states, while project hygiene was improved by untracking compiled CSS files and adding new SVG icons for a cleaner repository.

## 🚀 LatestUpdates (March 7, 2026)

**By Nora**
Refactored the bottom navigation to resolve icon scaling issues and improve UI responsiveness. Replaced the previous layout with a CSS Grid-based system that overlays outline and filled icons within the same cell, ensuring perfect alignment during transitions. Visual size discrepancies for the Home and Search filled icons were corrected using specific transform: scale() adjustments to compensate for SVG geometry differences. Additionally, implemented a Spotify-style glassmorphism effect on the footer using backdrop-filter: blur(), removed the default checked state from the Home tab to prevent pre-filled icons on refresh, and optimized the overall codebase by introducing reusable SCSS mixins for flexbox, glass effects, and positioning.

## 🚀 LatestUpdates (March 8, 2026)

**By Nora**
Today’s progress focused on refactoring the music player and navigation for better accessibility and UI precision. I adopted a component-based architecture, breaking down the UI into modular sections and managing them through dedicated SASS partials for cleaner, more maintainable code.

I replaced generic containers with semantic HTML5 (such as <section>, <figure>, and <time>) and implemented a CSS-only expansion using the "checkbox hack" to eliminate JavaScript dependency. The playback bar now features a dynamic SASS-managed marquee animation for long titles and a custom-styled <input type="range"> for a sleek seek bar. Additionally, I optimized the bottom navigation using CSS Grid to fix icon scaling issues, applied a glassmorphism effect via backdrop-filter, and streamlined the entire codebase with reusable SCSS mixins.
