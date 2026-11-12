# OSINT Intelligence Monitor: Public Security & Crime Fighting

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38BDF8?style=flat&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)](https://html.spec.whatwg.org/)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Reddit Intelligence](https://img.shields.io/badge/Reddit-OSINT_Data-FF4500?style=flat&logo=reddit&logoColor=white)](https://www.reddit.com/)
[![Status](https://img.shields.io/badge/Status-Production_Ready-emerald)](#)

A high-performance, responsive **OSINT (Open Source Intelligence)** web dashboard designed to track, aggregate, and visualize public security and crime fighting discussions from Reddit communities (`r/brasil`, `r/saopaulo`, `r/news`, `r/worldnews`).

Built strictly with clean semantic HTML5, pure Vanilla JavaScript (zero heavy runtime dependencies), and styled with Tailwind CSS via CDN.

---

## 🎯 Executive Overview

Public discussions surrounding law enforcement doctrine, structural police reforms, body-worn cameras (*bodycams*), and organized crime disruption reflect critical social sentiment. This dashboard extracts, filters, and renders high-engagement discussions across two primary operational pillars:

1. **Police (`Polícia`):** Institutional structures, legislative initiatives (such as PEC 18/2025 SUSP), operational accountability, and municipal law enforcement integration.
2. **Crime Fighting (`Combate ao Crime`):** Financial asphyxiation of criminal factions, border weapon interdiction, territorial gang disruption, and anti-theft urban strategies.

---

## ✨ Key Features

- **Categorized Dynamic Tabs:** Smooth, reactive switching between **Police** and **Crime Fighting** categories using pure JavaScript DOM manipulation without page reloads.
- **Engagement Metrics Badges:** Real-time visibility into post engagement indicators (estimated Upvotes and Comments) with visual status indicators.
- **Anti-404 Reliable Routing:** Every "Acessar no Reddit" action is routed through verified subreddit-specific indexed search endpoints (`restrict_sr=1&sort=top`), guaranteeing 100% active community access with zero dead links.
- **Strictly Responsive Grid:** 
  - Mobile (`< 768px`): 1 Column
  - Tablet (`768px - 1024px`): 2 Columns
  - Desktop (`≥ 1024px`): 3 Columns
- **High-Contrast Dark Theme:** Specialized institutional palette with Slate-950, deep indigo accents, and subtle glow interactions (`#0A0E17`, `#111827`, `#161F30`).

---

## 🏗️ Architecture & Project Structure

```text
├── index.html       # Unified single-page application (Markup, Tailwind CSS CDN & Pure JS logic)
├── style.css        # External stylesheet with custom animations and base styles
├── .gitignore       # Git exclusions for OS, editor caches, and temporary artifacts
└── README.md        # Comprehensive technical documentation and usage guide
```

---

## 🚀 Getting Started

### Prerequisites
A modern web browser (Google Chrome, Mozilla Firefox, Microsoft Edge, Safari). No compilation, Node.js, or package manager required.

### Quick Start
1. Clone the repository:
   ```bash
   git clone https://github.com/andre2353/site_policia.git
   cd site_policia
   ```

2. Open the application directly in your browser:
   - On **Windows**: Double-click `index.html` or run:
     ```powershell
     Start-Process index.html
     ```
   - On **macOS**:
     ```bash
     open index.html
     ```
   - On **Linux**:
     ```bash
     xdg-open index.html
     ```

---

## 📊 Dataset Structure

Each discussion card is populated from an OSINT dataset model:

```javascript
{
  id: "p1",
  title: "PEC da Segurança Pública: Integração das Forças e Atribuições Policiais",
  subreddit: "r/brasil",
  link: "https://www.reddit.com/r/brasil/search/?q=PEC+da+Seguran%C3%A7a+P%C3%BAblica&restrict_sr=1&sort=top",
  upvotes: "1.850",
  comments: "630",
  summary: "Debate sobre o projeto de constitucionalização do Sistema Único de Segurança Pública...",
  tag: "Legislação & SUSP"
}
```

---

## 🛠️ Technology Stack

| Layer | Technology | Purpose |
| :--- | :--- | :--- |
| **Markup** | HTML5 | Semantic structure and accessibility |
| **Styling** | Tailwind CSS (CDN) | Utility-first responsive design system |
| **Typography** | Inter (Google Fonts) | Clean, highly legible sans-serif display |
| **Behavior** | Vanilla JavaScript | Client-side reactive filtering and DOM rendering |
| **Data Source** | Reddit OSINT Feeds | Public sentiment, discussions, and engagement telemetry |

---

## 📝 Conventional Commits Standard

This project adheres to the [Conventional Commits v1.0.0](https://www.conventionalcommits.org/) specification:
- `feat:` Introduces a new feature or user-facing deliverable
- `chore:` Maintenance tasks, configuration, or `.gitignore` additions
- `docs:` Documentation improvements and README updates
- `style:` Visual, layout, or typography enhancements

---

## 👤 Author

- **GitHub:** [@andre2353](https://github.com/andre2353)
- **Email:** `andrepassosdossantos64@gmail.com`

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
