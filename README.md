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

**By Lana:**
Dixit-Spotify: Home Section Architecture
By Lana Tcholaria 

This project is a high-fidelity music streaming interface built with a mobile-first approach, focusing on fluid responsiveness, modular SCSS architecture, and interactive UI components.

:tools: Project Architecture
I was responsible for the core structure and styling of the Home Section, ensuring a seamless transition between various mobile viewports and desktop layouts. The codebase has been fully refactored from a monolithic stylesheet into a component-based design system.

:star2: Key Technical Features
1. Algorithmic Theme Engine
I transitioned from manual CSS styling to a logic-driven SASS architecture. By implementing dynamic @for loops combined with SASS Interpolation (#{$i}), I automated the theme assignment for over 20 unique album components.

2. Parallel Logic Execution
Within the _home-loops.scss partial, I engineered parallel loops that simultaneously manage:

Metadata Typography: Mapping unique color tokens to album subtitles.

Multi-layered Background Effects: Automating background-color and opacity for stacked album cover wrappers.

3. Fluid Responsive Scaling
I implemented a custom linear interpolation formula using clamp() and calc() within the $card-dimensions map. This ensures that cards scale perfectly from 15rem to 25rem without excessive media queries.

4. Pure CSS Interactivity
I engineered the "Customize Feed" menu using the Checkbox Hack (:checked ~ selector). This allows for a smooth, hardware-accelerated 1s slide-in animation from the bottom on mobile devices without any JavaScript overhead.

:bulb: Challenges & Solutions (By Lana)
One of the primary challenges was managing the Stacking Context within the .home container. Initially, decorative background elements were disappearing under the parent's background color. I resolved this by re-calibrating the z-index hierarchy and ensuring that each overlapping component exists within a stable stacking context.

_home-loops.scss: Houses all algorithmic styling and theme mapping.

_recent-played.scss: Encapsulates mobile-specific grid logic and responsive visibility.

_home-nav.scss: Isolates navigation, hover effects, and the icon-toggle system.

Refactoring Logs: Every major structural change, such as the isolation of home-loops.scss, was documented to ensure that the project's evolution is clear to other developers. This reflects a professional "Creator" mindset, where the code isn't just written, but managed with precision and clarity.
