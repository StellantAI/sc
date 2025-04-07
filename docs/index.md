# SC Design System

**SC** (Stellant Components) is the official UI design system developed by [StellantAI](https://stellantai.org) for building responsive, AI-native enterprise SaaS applications.

SC is a flexible, modular design system built using:
- ⚙️ **Vanilla JavaScript** and **Syncfusion EJ2** components
- 🎨 **Material UI-inspired** theme
- 📐 Responsive layouts for web, mobile, tablet with **Bootstrap 5.3 utility classes**
- 🧠 Forward-compatible with **AI-augmented** and **in-app UI generation**
- Chat UI layouts 
- App dashboard layouts
- Centralized UI resources: components, theme, styles, design, design tokens and CSS

---

## 🌟 Purpose

SC provides a unified visual language and component library for all StellantAI products, starting with our Clinical Quality Management SaaS solution. It is designed to work across:

- 💻 Web (Desktop)
- 📱 Mobile
- 📲 Tablet
- 🧠 AI-driven chat and in-app UI builders

---

## 📁 Project Structure

\`\`\`
sc/
├── ui-system/              # Tokens, themes, and reusable components
│   ├── tokens/             # JSON and SCSS-based design tokens
│   ├── components/         # Vanilla JS wrappers and styling
│   └── styles/             # Global styles, SC theme, layout utilities
├── docs/                   # Markdown docs for MkDocs site
│   ├── index.md
│   ├── tokens.md
│   ├── responsive-guidelines.md
│   └── components/
├── mkdocs.yml              # Documentation site configuration
└── README.md
\`\`\`

---

## 🚀 Features

- ✅ **Responsive-first grid system** (12-column layout at 1440px with 1280px content width)
- 🎨 **Design tokens** for color, typography, spacing (JSON + SCSS)
- 🧩 **Syncfusion EJ2 Vanilla JS components** with SC theme styling.  Syncfusion is a licensed product. This project includes references to syncfusion CDN and node_modules, but no license is to syncfusion is implied or offered.   Please contact syncfusion for licensing questions at:  [https://ej2.syncfusion.com/documentation/introduction](https://ej2.syncfusion.com/documentation/introduction)
- 🧠 **AI agent-compatible UI** via structured metadata
- ✨ **Styled using Figma + Syncfusion UI kits** for designer-developer collaboration

---

## 📐 Design & Layout Guidelines

| Form Factor | Recommended Size | Grid Columns | Notes |
|-------------|------------------|--------------|-------|
| Mobile      | 390×700          | 4–6          | Safe for most smartphones |
| Tablet      | 768×960 (portrait) | 8          | Standard iPad dimensions |
| Web (Desktop) | 1440×840       | 12           | Ideal for MacBook & HD screens |

See the full responsive guide in [`docs/responsive-guidelines.md`](./docs/responsive-guidelines.md).

---

## 📘 Documentation

SC uses [MkDocs](https://www.mkdocs.org/) with the [Material for MkDocs theme](https://squidfunk.github.io/mkdocs-material/) for documentation.

📖 Access docs locally:
\`\`\`bash
pip install mkdocs-material
mkdocs serve
\`\`\`

---

## 🎨 Figma Kits

SC is designed using Syncfusion's [Material 3 Figma UI kits](https://ej2.syncfusion.com/documentation/appearance/figma/), extended with StellantAI brand tokens and components. Designers should sync their libraries via Figma team assets.

---

## 🛠 Getting Started

Coming soon:
- `install.md` for setup instructions
- Component API usage examples
- Theme integration for Syncfusion EJ2 Vanilla

---

## 🤝 Contributing

Contributions from designers, developers, and UX engineers are welcome! Please review the [contributing guide](CONTRIBUTING.md) (to be added) and open a pull request.

---

## 📄 License

MIT License © 2025 StellantAI. See `LICENSE` for full terms.

---

## 🌐 Links

- GitHub: [github.com/StellantAI/sc](https://github.com/StellantAI/sc)
- Org Site: [stellantai.org](https://stellantai.org) *(coming soon)*