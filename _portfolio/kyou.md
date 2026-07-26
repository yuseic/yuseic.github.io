---
title: "KYOU (今日): High-End Generative Art & Digital Ritual PWA"
excerpt: "A 0-to-1 AI-assisted generative art PWA translating ancient GanZhi time coordinates into a daily glowing electric-ink mosaic ritual. Showcasing 0-1 product design, luxury aesthetic curation, and full-stack AI-assisted engineering."
collection: portfolio
header:
  teaser: "kyou/hero_demo.png"
---

**KYOU** (今日, *Today*) is a mobile-first, daily generative art Progressive Web App (PWA) that translates cosmological time coordinates (GanZhi, Five Elements) into a shared, deterministic digital ritual. 

Designed and engineered from scratch (0-to-1) using AI-assisted pair programming, KYOU reimagines traditional calendar systems into a high-end, contemplative visual experience.

---

## 🎨 Visual Artifact Showcase

### 1. Daily Energy Mosaic Hero (每日能量场主视觉)
The central visual engine calculates the daily Heavenly Stems and Earthly Branches (e.g., *Xin-Chou* 辛丑) and renders an interactive, 160-column mosaic electric grid field.

![KYOU Generative Energy Field Demo](/images/kyou/hero_demo.png)

*Figure 1: High-saturation Peking-Opera mask neon palette (Emerald Green for Wood, Vermilion Red for Fire, Golden Amber for Earth, Oceanic Blue for Water, Titanium Silver for Metal) flowing in dynamic wave interference patterns driven by Five Elements generative relationships.*

### 2. Mobile Digital Share Card (移动端艺术分享卡)
Users can export a high-resolution, seed-based share card with deterministic daily artwork, stylized GanZhi calligraphy, and non-predictive poetic reflection.

![KYOU Mobile Share Card](/images/kyou/share_card.png)

*Figure 2: Deterministic, seed-based share card generator integrated with native Web Share API for frictionless mobile sharing.*

---

## 🚀 Key Capabilities Highlighted

### 1. 0-to-1 Product Development & Vision (从零到一开发与产品定义)
* **Product Constitution ("Show, Don't Predict"):** Positioned against traditional fortune-telling/divination apps that exploit user anxiety. KYOU presents time as an entry point for daily presence and mindful contemplation.
* **Agile Pivot & Brand Iteration:** Rapidly evolved the product identity from an initial "quiet monochrome ink" prototype into a bold "High-End × Tradition" (高端 × 传统) digital neon ritual (*kyou*), validating product-market-fit for Gen-Z & luxury digital collectors.
* **End-to-End Delivery:** Managed the complete product lifecycle: product vision $\rightarrow$ mathematical data translation $\rightarrow$ custom WebGL/Canvas engine $\rightarrow$ PWA distribution $\rightarrow$ social share virality loop.

### 2. Design Excellence & Luxury Aesthetics (顶级 0-1 视觉设计与审美落地)
* **Peking-Opera Neon Palette:** Spec'd a custom color theory mapping Five Elements to ultra-saturated, high-contrast neon hues inspired by Peking Opera face painting and Chinese lacquerware set against a pitch-black canvas (`#050508`).
* **Micro-Interactions & Spatial Hierarchy:** Designed fluid particle physics, organic wave turbulence, and clean dark-mode spatial layouts to create an immersive, meditative interface.
* **Deterministic Reproducibility:** Every calendar date globally maps to a unique, 100% reproducible generative artwork seed.

### 3. AI-Assisted Engineering & System Architecture (AI 辅助全栈工程与性能调优)
* **Modular Architecture with LLM Pair-Programming:** Partnered with Claude/AI to split complex single-file prototypes into clean ES6 modules (`data.js`, `elements.js`, `electric-field.js`, `shichen.js`, `share-card.js`, `main.js`).
* **Algorithmic Performance Optimization:** Diagnosed a severe 60fps rendering bottleneck caused by thousands of per-cell `ctx.shadowBlur` invocations. Refactored the particle render loop into an offscreen-canvas Gaussian blur layer (离屏发光合成层), slashing GPU/CPU frame times by **90%+** while preserving glowing neon bloom.
* **Automated Daily Pipeline & Offline PWA:** Integrated `lunar-javascript` into an automated daily node script (`scripts/generate-daily.js`) with time-zone enforcement (`Asia/Ho_Chi_Minh`), paired with Service Worker caching for instant offline PWA loading.

---

## 🛠️ System Architecture

1. **Data Layer (`lunar-javascript`):** Ingests daily astronomical & Ganzhi coordinates.
2. **Translation Engine (`elements.js`):** Maps Stems & Branches五行 relationships (generating/overcoming) into color palettes, particle density, and flow velocity.
3. **Canvas Hero (`electric-field.js`):** Renders the real-time mosaic electric field with offscreen blur compositing.
4. **Export & Social Layer (`share-card.js`):** Generates high-res image cards using seed-based RNG (`rand()`) for Web Share API.

---

## 💻 Tech Stack

* **Core:** Vanilla JavaScript (ES6+), HTML5 Canvas 2D, Vanilla CSS (Design Tokens)
* **Libraries & PWA:** `lunar-javascript`, PWA Service Workers, Web Share API
* **Engineering Tools:** AI Pair Programming (Claude / Cursor), Node.js Build Runner
