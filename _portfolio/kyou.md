---
title: "KYOU: Algorithmic Time & Generative Art Digital Ritual"
excerpt: "A mobile-first, daily generative art PWA that translates cosmological calendar data (GanZhi, Five Elements) into a shared, contemplative digital ritual."
collection: portfolio
---

**Objective:** To design and implement **KYOU** (今日, Japanese for "Today")—a digital ritual app that translates ancient Eastern time systems (GanZhi, Five Elements) into daily, deterministic generative artworks. Rather than using temporal data for divination or fortune-telling, KYOU presents time as an entry point for daily presence and contemplation.

### The Philosophy: Observing the Present over Divination
Traditional calendar and astrology apps focus on "divining" or "predicting" the future, feeding user anxiety in the attention economy. KYOU operates under a strict **Product Constitution**:
*   **Show, Don't Predict:** The application presents "what today is" (e.g., *Bingwu* day) rather than "what will happen" or "what to do."
*   **Encourage Presence:** The UI utilizes slow transitions, micro-animations, and large, intentional white spaces (留白) designed to calm and ground the user.

### System Architecture: Data to Aesthetics
KYOU translates cyclical calendar coordinates into digital art through a structured pipeline:

1.  **Astronomical & Calendar Ingestion (Data Layer):**
    *   Integrates the `lunar-javascript` engine to calculate the precise Heavenly Stems, Earthly Branches, and Five Elements configurations for the current day.
    *   Applies a strict timezone enforcement (`Asia/Ho_Chi_Minh`) on the generation runner, ensuring all global users share the exact same temporal coordinates for a given calendar date.
2.  **Cosmological Mapping Engine (Translation Layer):**
    *   Extracts the daily Stems and Branches and computes their Five Elements balance (Wood, Fire, Earth, Metal, Water).
    *   Translates these energy states into visual design parameters (color hue, saturation, contrast, particle density, composition, and dynamic flow velocity).
    *   Generates a deterministic seed based on the date, guaranteeing that the daily artwork is reproducible and identical for every user globally.
3.  **Generative Presentation (Rendering Layer):**
    *   Renders abstract visual systems based on the translated parameters (e.g., "Neon Ink", "Song Painting Circuits", "Quantum Seals").
    *   Pairs the artwork with an open-ended, non-prescriptive original text phrase that encourages subjective interpretation.

### Technical Implementation
*   **Lightweight & Deployable:** Written in pure, dependency-free client-side JavaScript, HTML5 Canvas, and Vanilla CSS for maximum performance and easy static hosting.
*   **Progressive Web App (PWA):** Equipped with a `manifest.webmanifest` and custom `service-worker.js` for offline asset caching and seamless mobile-app launching.
*   **Frictionless Sharing:** Features a dynamic Canvas-based image generator that exports high-resolution sharing cards, integrated with the native Web Share API to directly prompt mobile device share sheets.

---
**Tech Stack:** JavaScript (ES6+), HTML5 Canvas, Vanilla CSS, `lunar-javascript`, PWA (Service Workers), Web Share API.
