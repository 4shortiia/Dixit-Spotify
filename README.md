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
Music Platform :headphones:
This project is a high-fidelity music streaming interface built with a mobile-first approach, focusing on fluid responsiveness and interactive UI components.

:tools: Project Architecture (Home Section - By Lana)
I was responsible for the core structure and styling of the Home Section, ensuring a seamless transition between various mobile viewports and initial desktop layouts.

:star2: Key Technical Features (By Lana)
Fluid Responsive Scaling: I implemented a custom linear interpolation formula using clamp() and calc() within the $card-dimensions map. This ensures that the recent-played cards scale perfectly from 15rem (at 320px) to 25rem (at 700px) without the need for excessive media queries.

Pure CSS Bottom Sheet Interaction: I engineered the customize-feed aside menu using the Checkbox Hack (:checked ~ selector). This allows for a smooth, hardware-accelerated 1s slide-in animation from the bottom on mobile devices, achieving complex interactivity without any JavaScript overhead.

Advanced Layering & Stack Effect: For the album sections, I designed the @mixin cover_wrapper. This mixin uses z-index layering and relative/absolute positioning to create a "stacked" folder-tab effect behind album covers, adding significant visual depth to the UI.

Mobile-First Breakpoint Strategy: I established a clear separation between mobile and desktop styles with a 800px breakpoint. Above this threshold, I managed layout cleanup by hiding mobile-specific sections (recent-played) to prepare for the desktop-exclusive grid restructuring.

:art: Design Systems & SCSS (By Lana)
Semantic Color Mapping: I developed a detailed color system for dynamic paragraph colors ($p-purple, $p-mint, etc.) and applied them using the :nth-child pseudo-selector logic to match specific album aesthetics.

Modular Mixins: All core components are built using reusable mixins (@mixin btn-reset, @mixin horizontal-scroll, @mixin album-cards), making the codebase highly maintainable and DRY (Don't Repeat Yourself).

Glassmorphism & Gradients: I applied complex linear-gradient backgrounds with high-opacity alpha channels to create a modern, immersive "Dark Mode" experience.

:bulb: Challenges & Solutions (By Lana)
One of the primary challenges was managing the Stacking Context within the .home container. Initially, decorative background elements were disappearing under the parent's background color. I resolved this by re-calibrating the z-index hierarchy and ensuring that each overlapping component exists within a stable stacking context.   

Custom Color Mapping for Album Stacks (By Lana): I implemented a unique visual identity for both the "Your Top Mixes" and "Made For You" sections. By manually mapping specific hex codes to each album's background layers using :nth-child selectors, I created a dynamic "shuffle" effect that harmonizes with each individual album's artwork.

Layered Transparency Logic: To achieve a realistic depth effect, I utilized a dual-opacity system (opacity: 0.15 for the back layer and opacity: 0.3 for the middle layer). This creates a sophisticated, translucent stacking effect that mimics a physical collection of vinyl or CDs.

Section Isolation: Each content block is strictly scoped within its parent class to ensure that the color palettes remain unique and do not interfere with other horizontal scroll components.