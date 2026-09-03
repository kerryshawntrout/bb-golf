# ⛳ Brilliantly Boring Golf

> **Consistency over complexity.** A lightweight, mobile-first Progressive Web App (PWA) designed to track course management, scoring zone metrics, and short-game execution without unnecessary fluff.

---

## 📌 Overview

**Brilliantly Boring Golf** focuses on the core metrics that actually lower scores. Instead of tracking traditional stats like Fairways in Regulation (FIR) or Greens in Regulation (GIR) that often reward risky play, this app emphasizes **Scoring Zone Regulation (SZ)**, **Up & Down Execution**, **Putting Proximity**, and **Penalty Avoidance**.

Built as a single-page PWA, it works offline on the course, saves round progress in real-time, and generates personalized practice plans based on your last 5 rounds.

---

## ✨ Key Features

* **Scoring Zone & Up/Down Metrics:**
  * **Strokes to SZ:** Record shots required to reach your target scoring zone (typically 80–120 yards out).
  * **Strokes SZ to Green:** Measure short-game efficiency from inside the scoring zone.
  * **Up & Down in 3:** Track conversion rates from inside the scoring zone to the hole in 3 strokes or fewer.
* **Putting Proximity & Performance:**
  * Track total putts, first putt distance (in paces), and first putt finish proximity (inside 4 ft).
* **Par & Penalty Tracking:**
  * Dynamic par alignment (Par 3, 4, 5) with automatic scoring zone baseline suggestions.
  * Penalty stroke counter to highlight risk management flaws.
* **Mid-Round Draft Autosave:**
  * Auto-saves hole-by-hole data to `localStorage`. Resume in-progress rounds seamlessly if the browser refreshes or phone turns off.
* **Smart Practice Plan Generator:**
  * Analyzes your **last 5 rounds** to pinpoint your weakest operational bottleneck (Approach, Short Game, or Lag Putting).
* **CSV Export & Local History:**
  * Keep full ownership of your data with one-click CSV exporting for external analysis.
* **Offline PWA Support:**
  * Fast loading with service worker caching for offline use on remote courses.

---

## 🛠️ Application Structure

```text
.
├── index.html          # Main application logic, UI structure, and inline styles
├── manifest.json       # PWA manifest (app icons, theme colors, display modes)
├── service-worker.js   # Service worker for offline asset caching
└── README.md           # Project documentation
