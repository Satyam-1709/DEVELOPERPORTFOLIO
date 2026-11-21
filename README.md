<div align="center">

# 🚀 DevPortfolio Builder

### *A modern, full-featured developer portfolio & case-study builder — no frameworks, no build tools, just the web.*

[![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge)](https://github.com/Satyam-1709/DEVELOPERPORTFOLIO)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![License](https://img.shields.io/badge/License-MIT-purple?style=for-the-badge)](LICENSE)
[![Zero Dependencies](https://img.shields.io/badge/Dependencies-Zero-blue?style=for-the-badge)](https://github.com/Satyam-1709/DEVELOPERPORTFOLIO)

</div>

---

## 📌 Table of Contents

- [About the Project](#-about-the-project)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [Getting Started](#-getting-started)
- [How to Use](#-how-to-use)
- [Templates](#-templates)
- [Contributing](#-contributing)
- [License](#-license)

---

## 💡 About the Project

**DevPortfolio Builder** is a fully client-side web application that empowers developers to create stunning, personalized portfolio websites — complete with structured project case studies — without writing a single line of code.

The app stores all data in `localStorage`, requires **zero backend**, and exports a **single standalone `.html` file** you can deploy anywhere: GitHub Pages, Netlify, Vercel, or any static host.

> Built with pure **Vanilla JavaScript (ES6+)**, **Semantic HTML5**, and **modular CSS3** — no frameworks, no bundlers, no build steps.

---

## ✨ Features

<details>
<summary><strong>🔐 Authentication System</strong></summary>

- Full **Login & Registration** flow with real-time password strength metering
- **"Try Demo — Skip Sign In"** mode for rapid evaluation
- Client-side **auth guard** protecting all app pages
- Persistent session via `localStorage`

</details>

<details>
<summary><strong>📊 Dashboard</strong></summary>

- Dynamic **user greeting** with live stats:
  - Total projects, skill count, profile completeness %, active template
- Interactive **setup checklist** with progress tracking
- **Recent activity feed** showing latest case-study updates

</details>

<details>
<summary><strong>👤 Personal Information Editor</strong></summary>

- Full profile customization: Name, Title, Bio, Email, Phone, Location, Website
- Social links management (GitHub, LinkedIn, Twitter, etc.)
- Dynamic **tag-based skill manager** with 35+ preset suggestions
- **Education & Work Experience** list managers with CRUD support
- **Debounced auto-save** with live visual feedback indicator

</details>

<details>
<summary><strong>🗂️ Project & Case-Study Builder</strong></summary>

- Full **CRUD operations** with instant search & duplicate tools
- Structured case study sections:
  - **Overview** — Title, tagline, technology tags, featured badge
  - **Case Study Breakdown** — Problem statement, solution architecture, key features, challenges & outcomes
  - **Media & Links** — Screenshot preview, Demo URL, GitHub link

</details>

<details>
<summary><strong>🎨 Template Gallery & Live Customizer</strong></summary>

- **3 Distinct Portfolio Templates:**

| Template | Style |
|----------|-------|
| `Aurora` | Dark gradient with glassmorphism & glow effects |
| `Minimal` | Clean, modern, high-contrast light typography |
| `Neon` | Cyberpunk terminal-inspired with glowing accents |

- **Live Editor:** Real-time color pickers, Google Font switcher, section visibility toggles
- **Responsive preview** — toggle between Desktop, Tablet & Mobile viewports

</details>

<details>
<summary><strong>📤 One-Click Export</strong></summary>

- Download a **self-contained `.html` file** ready to deploy
- **Copy source** directly to clipboard
- Works on GitHub Pages, Vercel, Netlify, or any static host

</details>

---

## 🛠️ Tech Stack

| Category | Technology |
|----------|-----------|
| **Structure** | HTML5 (Semantic) |
| **Styling** | CSS3 with Custom Properties (Variables) |
| **Logic** | Vanilla JavaScript (ES6+) |
| **Storage** | Browser `localStorage` with custom reactive event bus |
| **Fonts** | Google Fonts (Inter) |
| **Build Tools** | None — zero config |

**CSS Architecture (Modular):**

```
css/
├── variables.css    → Design tokens, color palette, spacing scale
├── reset.css        → Normalize & base styles
├── layout.css       → App shell, sidebar, responsive grid
├── components.css   → Reusable UI components (cards, buttons, badges)
├── forms.css        → Form elements and input styles
├── dashboard.css    → Dashboard-specific layout
└── animations.css   → Keyframe animations & transitions
```

---

## 📁 Project Structure

```
DEVELOPERPORTFOLIO/
│
├── index.html                    # Main Dashboard (entry point)
│
├── css/
│   ├── variables.css             # CSS custom properties & design tokens
│   ├── reset.css                 # Base reset & normalize
│   ├── layout.css                # App shell, sidebar, main layout
│   ├── components.css            # UI component styles
│   ├── forms.css                 # Input, select, textarea styles
│   ├── dashboard.css             # Dashboard page styles
│   └── animations.css            # CSS keyframe animations
│
├── js/
│   ├── core/
│   │   ├── auth.js               # Authentication & session management
│   │   ├── store.js              # Reactive localStorage data store
│   │   ├── router.js             # Client-side page routing
│   │   ├── theme.js              # Theme switcher (dark/light)
│   │   └── utils.js              # Shared utility functions
│   ├── pages/                    # Page-specific controllers
│   └── templates/                # Standalone portfolio template renderers
│
├── pages/
│   ├── auth.html                 # Login / Sign-up page
│   ├── personal-info.html        # Profile editor
│   ├── project-builder.html      # Case-study builder
│   ├── template-gallery.html     # Template selector
│   ├── live-editor.html          # Live customizer & preview
│   └── portfolio.html            # Full portfolio viewer & exporter
│
└── Sameera-UIUX/
    ├── PortfolioDesign.jsx        # UI/UX design reference (React component)
    ├── PortfolioDesign.css        # Design reference styles
    └── README.md                  # UI/UX design notes
```

---

## 🚀 Getting Started

### Prerequisites

- Any modern browser (Chrome, Firefox, Edge, Safari)
- No Node.js, npm, or build tools required!

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/Satyam-1709/DEVELOPERPORTFOLIO.git

# 2. Navigate into the project
cd DEVELOPERPORTFOLIO

# 3. Open index.html in your browser
# Option A — Double-click index.html
# Option B — Use a local server:

# Using Python
python -m http.server 8000

# Using Node.js (npx)
npx serve .

# Using VS Code Live Server extension
# Right-click index.html → "Open with Live Server"
```

Then visit `http://localhost:8000` in your browser.

---

## 📖 How to Use

1. **Sign In or Try Demo** — Click "Try Demo — Skip Sign In" for instant access
2. **Fill Your Profile** — Go to *Personal Info* and add your details, skills, education & experience
3. **Build Your Projects** — Use the *Project Builder* to create detailed case studies
4. **Pick a Template** — Browse the *Template Gallery* and choose your style
5. **Customize It** — Open the *Live Editor* to tweak colors, fonts & layout
6. **Export** — Hit the export button to download your portfolio as a standalone `.html` file
7. **Deploy** — Upload to GitHub Pages, Netlify, Vercel, or any static host!

---

## 🎨 Templates

| Template | Mode | Style |
|----------|------|-------|
| **Aurora** | Dark | Glassmorphism, gradient glow, purple-blue palette |
| **Minimal** | Light | Clean typography, whitespace-focused, monochrome |
| **Neon** | Dark | Cyberpunk terminal aesthetic, neon green/pink accents |

---

## 🤝 Contributing

Contributions, issues and feature requests are welcome!

1. **Fork** the repository
2. **Create** your feature branch: `git checkout -b feature/AmazingFeature`
3. **Commit** your changes: `git commit -m 'Add some AmazingFeature'`
4. **Push** to the branch: `git push origin feature/AmazingFeature`
5. **Open** a Pull Request

---

## 📄 License

Distributed under the **MIT License**. See [`LICENSE`](LICENSE) for more information.

You are free to use, modify, and distribute this project for personal or commercial purposes.

---

<div align="center">

Made with ❤️ by [Satyam](https://github.com/Satyam-1709)

⭐ **Star this repo** if you found it helpful!

</div>
