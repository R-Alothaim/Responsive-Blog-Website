# Living the Simple Life

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Responsive](https://img.shields.io/badge/Responsive-Design-44cc11?style=for-the-badge)

A clean, responsive blog exploring minimalism and simple living. Built with semantic HTML5 and a modular CSS architecture, the site adapts seamlessly across desktop, tablet, and mobile viewports.

> **Live demo:** [https://r-alothaim.github.io/Responsive-Design/](https://r-alothaim.github.io/Responsive-Design/)

---

## Table of Contents

- [Features](#features)
- [Project Architecture](#project-architecture)
- [CSS Architecture](#css-architecture)
- [Pages](#pages)
- [Getting Started](#getting-started)
- [Browser Support](#browser-support)
- [Screenshots](#screenshots)
- [Credits](#credits)
- [License](#license)
- [Author](#author)

---

## Features

- **Modular CSS Architecture** -- styles split into six focused files for maintainability
- **CSS Custom Properties** -- centralized design tokens for colors, typography, and spacing
- **Responsive Design** -- fluid layout that adapts to any screen size using flexbox
- **Semantic HTML5** -- accessible markup with `<header>`, `<main>`, `<article>`, `<aside>`, `<footer>`
- **Accessibility** -- proper alt text, focus states, and semantic structure
- **Google Fonts** -- Lora (serif headings) and Ubuntu (sans-serif body)
- **Multi-Page Navigation** -- home, about, and recent posts pages with active-state indicators

---

## Project Architecture

```
Responsive-Design/
├── assets/
│   ├── css/
│   │   ├── reset.css          CSS reset / normalize
│   │   ├── variables.css      CSS custom properties (design tokens)
│   │   ├── base.css           Base element styles
│   │   ├── layout.css         Container, flexbox grid, header, footer
│   │   ├── components.css     Nav, articles, sidebar widgets, pop-up
│   │   └── responsive.css     All @media queries
│   ├── images/
│   │   ├── about-me.jpg
│   │   ├── deco.jpg
│   │   ├── food.jpg
│   │   ├── life.jpg
│   │   └── work.jpg
│   └── fonts/                 Reserved for future custom fonts
├── pages/
│   ├── about.html             Author bio and personal story
│   └── posts.html             Full listing of recent articles
├── index.html                 Home page with featured article
├── 404.html                   Custom error page
├── .editorconfig
├── .gitattributes
├── .gitignore
├── LICENSE
├── package.json
└── README.md
```

---

## CSS Architecture

Styles are loaded in a deliberate cascade order. Each file has a single responsibility:

| Order | File | Purpose |
|-------|------|---------|
| 1 | `reset.css` | Strips browser defaults for a consistent baseline |
| 2 | `variables.css` | Defines all design tokens (`:root` custom properties) |
| 3 | `base.css` | Applies default styles to bare HTML elements |
| 4 | `layout.css` | Structural containers, header, and footer |
| 5 | `components.css` | Reusable UI patterns -- nav, cards, widgets, pop-up |
| 6 | `responsive.css` | All media queries in a single location |

This ordering ensures specificity flows naturally: resets first, then tokens, then increasingly specific rules.

---

## Pages

| Page | Path | Description |
|------|------|-------------|
| Home | `index.html` | Featured article, recent post cards, and sidebar widgets |
| About | `pages/about.html` | Author background story with expandable post widget |
| Recent Posts | `pages/posts.html` | Complete listing of all blog articles |
| 404 | `404.html` | Friendly error page with navigation back to home |

---

## Getting Started

No build tools or dependencies are required. Open `index.html` directly in any modern browser.

```bash
# Clone the repository
git clone https://github.com/R-Alothaim/Responsive-Design.git
cd Responsive-Design

# Option A: open directly
open index.html

# Option B: use a local dev server with auto-reload
npm run dev
```

The `npm run dev` script starts [live-server](https://www.npmjs.com/package/live-server) on port 3000 with automatic browser reloading.

---

## Browser Support

| Browser | Version |
|---------|---------|
| Chrome | last 2 versions |
| Firefox | last 2 versions |
| Safari | last 2 versions |
| Edge | last 2 versions |

The site uses CSS custom properties and flexbox, which are supported in all modern browsers.

---

## Screenshots

_Screenshots coming soon._

---

## Credits

This project was built as part of the [Scrimba Responsive Web Design Bootcamp](https://scrimba.com/learn/responsive).

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Author

**R-Alothaim** -- [GitHub Profile](https://github.com/R-Alothaim)
