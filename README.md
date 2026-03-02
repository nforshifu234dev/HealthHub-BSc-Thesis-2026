<div align="center">

# 🏥 HealthHub

### *Hybrid Rule-Based Expert System for Symptom Triage with Multilingual Support*
#### *Equitable Healthcare Access in Nigeria — The HealthHub Framework*

---

![Status](https://img.shields.io/badge/Status-Completed%20%26%20Defended-brightgreen?style=for-the-badge)
![Platform](https://img.shields.io/badge/Platform-Android%20%7C%20iOS%20%7C%20PWA-blue?style=for-the-badge)
![Offline](https://img.shields.io/badge/Mode-Offline--First-orange?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-lightgrey?style=for-the-badge)

---

**🎓 B.Sc. (Hons) Computer Science (Information Systems) — Final Year Project, 2026**
**Babcock University | Department of Computer Science, School of Computing**

**Built by:**
[Nyuiring-yoh Rhagninyui Shifu-Nfor](https://github.com/nforshifu234dev) · [Ogbaji Olivia Chisom](https://github.com/nforshifu234dev)

**Supervised by:** *Mr. Opeyemi Adelowo*

---

*A project by **[NFORSHIFU234 Dev](https://github.com/nforshifu234dev)** · Powered by **NFORSHIFU LogicForge Ltd.***

</div>

---

## 📖 Overview

**HealthHub** is an **offline-first, multilingual mobile/PWA prototype** designed to deliver immediate, transparent, and safe symptom triage guidance in low-resource Nigerian settings — particularly rural areas challenged by poor connectivity and rich linguistic diversity.

The system targets common and endemic conditions (malaria, Lassa fever, etc.) and supports **English, Pidgin, Hausa, Yorùbá, and Igbo** through fully localized UI and symptom checklists — no internet required.

> 💡 *The goal is simple: bring accessible, trustworthy health guidance to every Nigerian — regardless of location, language, or data connection.*

---

## ✅ Implemented Features (MVP)

| Feature | Details |
|--------|---------|
| 🌍 **Multilingual Support** | Language selection UI + i18n via `react-i18next` (EN, Pidgin, Hausa, Yorùbá, Igbo) |
| 📋 **Symptom Input** | Pre-translated symptom checklists — no real-time NLP required |
| 🧠 **Transparent Triage Logic** | Rule-based engine (`json-rules-engine`) with NCDC/WHO-derived IF-THEN rules |
| 🚦 **Urgency Classification** | Four levels: `Low` / `Medium` / `High` / `Emergency` with advice & disclaimers |
| 📱 **Offline History** | Encrypted local storage of past triage sessions + basic wellness reminders |
| 🔒 **Secure Local Storage** | Expo SQLite (native) + localForage (web) — encrypted at rest |
| 📡 **Full Offline Operation** | Runs smoothly on mid-range Android & iOS devices, zero connectivity needed |

---

## 🚧 Planned for Future Versions

These features are **not part of the MVP** but are scoped for future development:

- 🤖 On-device lightweight NLP/LLM inference (e.g., distilled N-ATLaS variants)
- 🎙️ Voice input processing
- ☁️ Cloud sync for rule & content updates

---

## 🛠️ Tech Stack

```
📱 Frontend / App     →  React Native 0.75 + Expo SDK 51 (Android / iOS / PWA)
🌐 Multilingual       →  react-i18next (static JSON translations + checklists)
🧠 Triage Engine      →  json-rules-engine (explainable, rule-based)
💾 Local Storage      →  Expo SQLite (native) + localForage (web) — encrypted
📐 Diagrams           →  Draw.io
🎨 Styling            →  CSS / React Native StyleSheet
```

---

## 📁 Repository Structure

> ⚠️ **This repository contains academic documentation only.** The application source code is **not open-sourced**.

```
HealthHub-BSc-Thesis-2026/
├── 📄 docs/
│   └── HealthHub_Thesis_Full.pdf           # Final compiled thesis (PDF)
│
├── 📐 appendices/
│   └── chapter3_diagrams/                  # All 9 Draw.io diagrams (PNG + .drawio source)
│       ├── Figure_1_Incremental_Model.png
│       ├── Figure_2_MVP_Architecture.png
│       ├── Figure_3_Flowchart.png
│       └── ... (all others)
│
├── 📸 screenshots/                         # App UI screenshots
│   ├── language_selection.png
│   ├── symptom_checklist_yoruba.png
│   └── triage_emergency_igbo.png
│
├── 📄 README.md
└── 📜 LICENSE                              # MIT (docs & diagrams)
```

---

## 👀 How to View the Work

1. **📘 Thesis** — Download the full PDF from `/docs/HealthHub_Thesis_Full.pdf`
2. **📐 Diagrams** — Browse high-res architecture & flow diagrams in `/appendices/chapter3_diagrams/`
3. **📸 Screenshots** — See the live app UI in `/screenshots/`

---

## 📜 License

Documentation, diagrams, and screenshots are licensed under the **MIT License** — free to view, share, and cite with proper attribution.

> The application source code remains **private and proprietary**.

---

## 🤝 Contact & Collaboration

Interested in piloting, extending, or collaborating on HealthHub? We'd love to hear from you!

| | |
|---|---|
| 👨‍💻 **GitHub** | [@nforshifu234dev](https://github.com/nforshifu234dev) |
| 🐦 **X / Twitter** | [@nforshifu234dev](https://x.com/nforshifu234dev) |
| 🏢 **Organization** | [NFORSHIFU LogicForge Ltd.](https://github.com/nforshifu234dev) |

> 💬 Feel free to **open an issue** or reach out directly for academic inquiries, collaboration interest, or partnership opportunities.

---

<div align="center">


*Crafted with 💙 by **[NFORSHIFU234 Dev](https://github.com/nforshifu234dev)***
*© 2026 **NFORSHIFU LogicForge Ltd.** — All rights reserved.*

*Babcock University · Department of Computer Science · B.Sc. Computer Science (Information Systems)*

</div>

---
