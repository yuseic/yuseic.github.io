---
title: "Tomo (山海图鉴): Single-Player Personal Relationship Atlas iOS App"
excerpt: "A private, single-player native iOS app (SwiftUI + SwiftData + Supabase Edge Functions) that records relationships into a private 'Bazi Universe' mineral pigment atlas (山海图鉴 · 矿彩版). Combining privacy-first architecture, traditional calendar algorithms, and Chinese mineral pigment aesthetics."
collection: portfolio
order: 2
header:
  teaser: "tomo/teaser.png"
---

**Tomo** (山海图鉴 / 八字宇宙) is a private, single-player native iOS application that reimagines personal social relationships into a private, collectible mineral pigment universe (*山海图鉴 · 矿彩版*).

Instead of social feeds, public request flows, or cloud social graphs, Tomo provides a quiet personal observation post where users manually record significant people, their precise birth coordinates, and subjective relationship memories.

---

## 🎨 Visual & Aesthetic System (*山海图鉴 · 矿彩版*)

### 1. Parchment & Mineral Color Palette
Inspired by classical Chinese mineral pigment notes (*《山海经》"其阳多金，其阴多铁"*), Tomo abandons standard dark mode toggles in favor of a fixed, physical warm parchment texture (`#EFE4C8`) and ten fixed mineral pigment hues:

* 🌿 **Wood (木):** 石绿 (`#2F6B46` 甲) · 翠玉 (`#6B9A6F` 乙)
* 🔥 **Fire (火):** 朱砂 (`#B23B2C` 丙) · 银朱 (`#C9683F` 丁)
* 🌾 **Earth (土):** 赭石 (`#9A6A2E` 戊) · 黄土 (`#C99A4A` 己)
* ⚔️ **Metal (金):** 古铜 (`#8A6B3A` 庚) · 银白 (`#AB9F86` 辛)
* 🌊 **Water (水):** 玄青 (`#2F3F5A` 壬) · 石青 (`#486A86` 癸)

### 2. Single-Player "Show, Don't Predict" Philosophy
* **No Divination or Judgment:** Tomo strictly avoids fortune-telling, compatibility scoring, or unsolicited life advice. Bazi time coordinates serve purely as subjective visual anchors and relationship spectrum collectors.
* **Privacy-First Boundary:** Zero cloud accounts, zero cloud relationship storage. All personal records, notes, and relationship memories are encrypted and stored strictly on-device using iOS 17+ SwiftData.

---

## 🚀 Technical Architecture

1. **Native iOS App (`SwiftUI` + `SwiftData`):**
   * Built for iOS 17+ with SwiftData local persistence.
   * Custom minimalist ink gesture glyphs (`BeastGlyph`) and vector seal components.
2. **Stateless Calendar Conversion Service (`Supabase Edge Functions`):**
   * Serverless Deno Edge Function powered by `lunar-typescript`.
   * Accepts birth date, precise time, location, and IANA timezone to compute Four Pillars (四柱) and Day Master (日主).
   * Enforces 23:00 Zi-hour (子时) day-boundary advancing rules.
   * Completely stateless: zero user accounts, zero saved records on the server.

---

## 💻 Tech Stack

* **Client:** Native iOS 17+ (SwiftUI, SwiftData, Swift Concurrency)
* **Backend:** Supabase Edge Functions (Deno / TypeScript, `lunar-typescript`)
* **Design Tokens:** Chinese Mineral Pigments, Custom Typography (`Songti SC`), Custom Vector Glyphs
