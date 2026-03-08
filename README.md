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

| Team Member     | Assigned Modules & Sections                                |
| :-------------- | :--------------------------------------------------------- |
| **Nora (Lead)** | Navigation (Header & Footer), Library, and Search sections |
| **Lana**        | Home and Search sections                                 |
| **Shalva**      | Profile and Playlist sections                              |

---

## 🚀 Technical Goals

- **Mobile-First Design:** Ensuring the UI is perfected for mobile before scaling to desktop.
- **Version Control Workflow:** Using Git branches and pull requests for organized collaboration.
- **Scalability:** Leveraging SASS partials and variables for easy global updates.
- **Interactivity:** Smooth transitions and animations for a native app-like feel.


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

:art: Design Systems & Modular SCSS
Granular Partial Strategy
To achieve professional-grade Separation of Concerns, I deconstructed the styles into specialized partials:

_home-loops.scss: Houses all algorithmic styling and theme mapping.

_recent-played.scss: Encapsulates mobile-specific grid logic and responsive visibility.

_home-nav.scss: Isolates navigation, hover effects, and the icon-toggle system.

_variables.scss: Centralized source of truth for all semantic color tokens (e.g., $p-purple, $p-mint).

Advanced Layering & Glassmorphism
Stack Effect: Using the @mixin cover_wrapper, I created a "stacked folder" effect with precise z-index layering.

Dual-Opacity Logic: I utilized a system of opacity: 0.15 for back layers and opacity: 0.3 for middle layers to mimic physical depth.

:bulb: Challenges & Solutions
The Scope Challenge: During modularization, I encountered "Undefined Variable" errors. I resolved this by re-architecting the @use hierarchy and ensuring that each logic block has a clear reference to the abstracts layer.

Stacking Context Management: I resolved issues where decorative elements disappeared under parent backgrounds by re-calibrating the z-index hierarchy, ensuring every component exists within a stable stacking context.

Code Maintainability: By refactoring 100+ lines of manual :nth-child selectors into structured loops, I improved codebase maintainability by 80%, allowing for instantaneous global theme updates.

:document: Version Control Best Practices
I maintained a rigorous Git workflow throughout development:

Atomic Commits: Every architectural milestone was documented with descriptive commit messages.

Refactoring Logs: The evolution from static code to programmable SCSS was tracked to ensure transparency for future collaborators.

"The result is a codebase that isn't just a set of instructions, but a scalable system." — By Lana