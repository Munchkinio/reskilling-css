# Epixelab — Landing Page

A responsive marketing landing page for a digital startup agency. Built with plain HTML and CSS — no frameworks, no build tools.

---

## 🚀 How to Run

No installation or build step required.

1. Clone the repository:
   ```bash
   git clone https://gitbud.epam.com/Dzmitry_Braitsau/epixelab-landing.git
   cd epixelab-landing
   ```

2. Open `index.html` directly in your browser — or use a local dev server for a better experience:
   ```bash
   # Using VS Code Live Server extension — recommended
   # Or with npx:
   npx serve .
   ```

That's it. No `npm install`, no compilation.

---

## 📁 Project Structure

```
epixelab-landing/
├── index.html
├── css/
│   └── style.css
└── assets/
    └── images/
        ├── logo.svg
        ├── hero-man.png
        ├── hero-bg.png
        ├── play-button.svg
        ├── icon-design.svg
        ├── icon-video.svg
        ├── icon-marketing.svg
        ├── video-thumb.jpg
        ├── avatar-1..4.jpg
        ├── team-1..3.jpg
        └── envelope.png
```

---

## 🧩 Sections

| Section | Description |
|---|---|
| Header | Sticky navigation with logo, nav links, login/signup |
| Hero | Headline, CTA buttons, floating info cards |
| Services | Three service cards (Design, Video, Marketing) |
| Blocks | Split layout with a video thumbnail |
| Testimonials | 2×2 grid of client reviews |
| Team | Three team member cards with social links |
| Subscribe | Newsletter signup form |
| Footer | Links and copyright |

---

## 🛠 Technologies

- **HTML5** — semantic markup (`<section>`, `<article>`, `<nav>`, etc.)
- **CSS3** — custom properties (variables), CSS Grid, Flexbox, media queries
- **Google Fonts** — Mulish (400–900)
- **Font Awesome 6** — icons in team card social links

---

## 📱 Responsive Design

The layout is fully responsive with a single breakpoint at `768px`. On mobile:
- Navigation collapses (burger menu button shown; JS toggle not yet implemented)
- All multi-column grids switch to a single column
- Hero image floating cards reposition

---

## 📝 Notes & Known Issues

- **Burger menu** — the hamburger button is rendered but has no JS attached yet. Opening the mobile menu requires additional scripting.
- **Video playback** — the play button in the Blocks section is visual only; no video player is wired up.
- **Hero card positioning** — the floating cards use fixed pixel offsets (`bottom: 204px; right: 418px`) tied to the hero image size. This may need adjustment if the image changes.
- **Placeholder text** — several sections still contain Lorem Ipsum copy that should be replaced with real content.

---

## ✅ What Went Well

- CSS custom properties made the color system easy to maintain — changing the brand color requires updating one variable.
- Using CSS Grid for the main layout kept the responsive code clean without relying on a framework.

---

## 🔮 Possible Improvements

- Add JS for the mobile burger menu toggle
- Implement smooth scroll-spy to highlight the active nav link on scroll
- Replace fixed pixel positioning on hero cards with percentage-based values
- Add a simple CSS animation for the hero section on page load