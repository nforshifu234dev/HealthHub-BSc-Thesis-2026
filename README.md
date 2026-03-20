# 🏥 HealthHub
### Hybrid Rule-Based Expert System for Symptom Triage with Multilingual Support
**Equitable Healthcare Access in Nigeria — The HealthHub Framework**

[![Status](https://img.shields.io/badge/Status-Live%20PWA-brightgreen?style=for-the-badge)](https://healthhub.nforshifu234dev.com)
[![Platform](https://img.shields.io/badge/Platform-Android%20%7C%20PWA-blue?style=for-the-badge)](https://healthhub.nforshifu234dev.com/download)
[![Offline](https://img.shields.io/badge/Offline-100%25-orange?style=for-the-badge)](https://healthhub.nforshifu234dev.com)
[![License](https://img.shields.io/badge/Docs%20License-MIT-green?style=for-the-badge)](LICENSE)

---

🎓 **B.Sc. (Hons) Computer Science (Information Systems) — Final Year Project, 2026**  
Babcock University | Department of Computer Science, School of Computing

**Built by:** Nyuiring-yoh Rhagninyui Shifu-Nfor · Ogbaji Olivia Chisom  
**Supervised by:** Mr. Opeyemi Adelowo  
**A project by** NFORSHIFU234 Dev · **Powered by** NFORSHIFU LOGICFORGE LTD (RC: 9359228)

---

## 🌐 Live Demo

| Link | Description |
|---|---|
| [healthhub.nforshifu234dev.com](https://healthhub.nforshifu234dev.com) | Live PWA — works fully offline |
| [/how-it-works](https://healthhub.nforshifu234dev.com/how-it-works) | Full triage rule transparency — every IF-THEN rule, clinical rationale, and source |
| [/about](https://healthhub.nforshifu234dev.com/about) | Project background and academic context |
| [/download](https://healthhub.nforshifu234dev.com/download) | Android APK and platform downloads |

---

## 📖 Overview

HealthHub is an **offline-first, multilingual mobile/PWA prototype** designed to deliver immediate, transparent, and safe symptom triage guidance in low-resource Nigerian settings — particularly rural areas challenged by poor connectivity and linguistic diversity.

The system targets common and endemic conditions (malaria, Lassa fever, cholera, typhoid, and others) and supports **English, Pidgin, Hausa, Yorùbá, and Igbo** through fully localised UI and symptom checklists — no internet required after installation.

> **The goal:** bring accessible, trustworthy health guidance to every Nigerian — regardless of location, language, or data connection.

---

## 🔑 Key Contribution: Rule Safety Gate

A critical engineering contribution of this project is the implementation of a **false-positive safety gate** in the triage engine. During prototype testing, the initial rule set incorrectly triggered a Lassa fever emergency alert for fever + headache alone — a dangerously misleading result.

The corrected engine:
- Requires **haemorrhagic indicators** (bleeding, facial swelling, or deafness) alongside fever before escalating to Lassa emergency priority
- Implements `EMERGENCY_MIN_SYMPTOMS = 2`: emergency rules cannot fire on a single reported symptom
- Documents all 26 triage rules publicly at [/how-it-works](https://healthhub.nforshifu234dev.com/how-it-works)

---

## ✅ Implemented Features (MVP)

| Feature | Details |
|---|---|
| 🌍 **Multilingual Support** | Language selection + i18n via react-i18next (EN, Pidgin, Hausa, Yorùbá, Igbo) |
| 📋 **Symptom Input** | Pre-translated symptom checklists — no real-time NLP required |
| 🧠 **Transparent Triage Logic** | 26 clinically-derived IF-THEN rules with safety gate (NCDC/WHO/ICD-11 sourced) |
| 🚦 **Urgency Classification** | Four levels: Low / Medium / High / Emergency with advice and disclaimers |
| 🔍 **Explainability** | Every result traceable to a named rule and clinical source |
| 📱 **Offline History** | Encrypted local SQLite storage of past triage sessions |
| 🔒 **Privacy-First** | NDPR-compliant; all data stored on-device only |
| 📡 **Full Offline Operation** | Runs on mid-range Android and iOS; zero connectivity needed |

---

## 🚧 Planned for Future Versions

- 🤖 On-device lightweight NLP (distilled N-ATLaS variants via TensorFlow Lite)
- 🎙️ Voice input and speech-to-text processing
- ☁️ Optional cloud sync for rule updates
- 🏥 Integration with state primary healthcare boards and campus clinics

---

## 🛠️ Tech Stack

```
📱 Frontend / App     →  React Native 0.75 + Expo SDK 51 (Android / iOS / PWA)
🌐 Multilingual       →  react-i18next (static JSON translations + symptom checklists)
🧠 Triage Engine      →  Custom TypeScript rule evaluator with safety gate (ruleEngine.ts)
💾 Local Storage      →  Expo SQLite (native) + localForage (web) — encrypted
🔐 Auth               →  Custom AuthContext (authenticated + guest modes)
📐 Diagrams           →  Draw.io
🎨 Styling            →  React Native StyleSheet + NativeWind
```

---

## 📁 Repository Structure

> ⚠️ This repository contains **academic documentation only**. The application source code is proprietary to NFORSHIFU LOGICFORGE LTD and is not open-sourced.

```
HealthHub-BSc-Thesis-2026/
│
├── 📄 docs/
│   ├── HealthHub_Thesis_Revised.pdf         # Full revised thesis (PDF)
│   └── HealthHub_Thesis_Revised.docx        # Full revised thesis (Word)
│
├── 📐 appendices/
│   └── chapter3_diagrams/                   # All 9 Draw.io diagrams (PNG + .drawio)
│       ├── Figure_3.1_Incremental_Model.png
│       ├── Figure_3.2_MVP_Architecture.png
│       ├── Figure_3.3_Flowchart.png
│       ├── Figure_3.4_UseCase.png
│       ├── Figure_3.5_Sequence.png
│       ├── Figure_3.6_ERD.png
│       ├── Figure_3.7_DFD_Level0.png
│       ├── Figure_3.8_DFD_Level1.png
│       └── Figure_3.9_Component.png
│
├── 📸 screenshots/
│   ├── language_selection.png               # Language picker screen
│   ├── symptom_checklist_english.png        # Symptom input (English)
│   ├── symptom_checklist_yoruba.png         # Symptom input (Yorùbá)
│   ├── triage_result_emergency.png          # Emergency urgency result
│   ├── triage_result_high.png               # High priority result
│   └── triage_result_low.png                # Low priority / default result
│
├── 📄 README.md
└── 📜 LICENSE                               # MIT (docs and diagrams only)
```

---

## 👀 How to View the Work

| Resource | Location |
|---|---|
| 📘 Full Thesis (PDF) | `/docs/HealthHub_Thesis_Revised.pdf` |
| 📐 System Diagrams | `/appendices/chapter3_diagrams/` |
| 📸 App Screenshots | `/screenshots/` |
| 🔍 Triage Rules (Live) | [healthhub.nforshifu234dev.com/how-it-works](https://healthhub.nforshifu234dev.com/how-it-works) |
| 🌐 Live PWA | [healthhub.nforshifu234dev.com](https://healthhub.nforshifu234dev.com) |

---

## 📊 System Overview

```
User selects language
        ↓
User selects symptoms (localised checklist)
        ↓
ruleEngine builds a fact map
        ↓
Engine evaluates 26 IF-THEN rules (NCDC/WHO/ICD-11)
        ↓
Safety gate: emergency rules require ≥ 2 symptoms
        ↓
Priority sort: Emergency (4) > High (3) > Medium (2) > Low (1)
        ↓
Result rendered in the selected language
        ↓
Disclaimer displayed — "HealthHub is NOT a doctor"
        ↓
Session saved to an encrypted local SQLite
```

---

## 📜 License

Documentation, diagrams, and screenshots are licensed under the **MIT License** — free to view, share, and cite with proper attribution.

The application source code is **proprietary to NFORSHIFU LOGICFORGE LTD** and is not open-sourced.

**Academic citation:**
> Shifu-Nfor, N. R. Y. & Ogbaji, O. C. (2026). *Developing a Hybrid Rule-Based Expert System for Symptom Triage with Multilingual Support for Equitable Medical Care Access in Nigeria: The HealthHub Framework*. B.Sc. (Hons) Thesis, Department of Computer Science, Babcock University, Nigeria.

---

## 🤝 Contact and Collaboration

Interested in piloting, extending, or collaborating on HealthHub? We welcome academic enquiries, partnership interest, and pilot programme discussions.

| | |
|---|---|
| 👨‍💻 **GitHub** | [@nforshifu234dev](https://github.com/nforshifu234dev) |
| 🐦 **X / Twitter** | [@nforshifu234dev](https://x.com/nforshifu234dev) |
| 🌐 **Website** | [nforshifu234dev.com](https://nforshifu234dev.com) |
| 🏢 **Company** | [NFORSHIFU LOGICFORGE LTD](https://linkedin.com/company/nforshifu-logicforge-ltd) |
| 📧 **Email** | info@nforshifu234dev.com |

Open an issue or reach out directly for academic enquiries, collaboration, or partnership opportunities.

---

*Crafted with 💙 by NFORSHIFU234 Dev*  
*© 2026 NFORSHIFU LOGICFORGE LTD — All rights reserved.*  
*Babcock University · Department of Computer Science · B.Sc. Computer Science (Information Systems)*
