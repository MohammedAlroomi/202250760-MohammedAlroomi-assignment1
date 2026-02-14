# Technical Documentation

**Project:** Personal Portfolio Web Application
**Student:** Mohammed Alroomi (202250760)

---

## Architecture

A static single-page application with no backend or build tools, organized into three core files:

```
index.html       ← Structure and content
css/styles.css   ← All styling and theming
js/script.js     ← All interactivity
```

---

## HTML Structure

| Section | Description |
|---------|-------------|
| `<nav>` | Fixed navbar with logo, links, and theme toggle |
| `#hero` | Landing area with name, tagline, and terminal widget |
| `#about` | Personal intro, details, and achievement badges |
| `#projects` | Three project cards with images and tech tags |
| `#experience` | Timeline of internship, McKinsey program, and SAC role |
| `#contact` | Validated contact form and contact info |

---

## CSS

- **Theming:** CSS custom properties on `:root` for all colors. Dark/light switch by toggling a class on `<body>`.
- **Layout:** CSS Grid for two-dimensional sections (hero, projects, contact), Flexbox for one-dimensional flows (navbar, buttons).
- **Responsive breakpoints:** 900px (tablet), 640px (mobile — hamburger menu activates).
- **Fonts:** Sora (body), Space Mono (monospace accents) via Google Fonts.

---

## JavaScript Features

| Function | Purpose |
|----------|---------|
| `setGreeting()` | Shows morning / afternoon / evening / night based on local time |
| `initTheme()` | Toggles dark/light theme, saves preference to `sessionStorage` |
| `initNavbar()` | Adds shadow to navbar on scroll |
| `initHamburger()` | Opens/closes mobile nav menu |
| `initSmoothScroll()` | Smooth scrolling to sections on nav link click |
| `initScrollAnimations()` | Fade-in on scroll using `IntersectionObserver` |
| `initContactForm()` | Validates name, email, and message with inline error messages |

---

## File Reference

| File | Purpose |
|------|---------|
| `index.html` | Main HTML document |
| `css/styles.css` | All styles |
| `js/script.js` | All JavaScript |
| `assets/images/` | Project placeholder images |
| `docs/ai-usage-report.md` | AI usage documentation |
| `docs/technical-documentation.md` | This file |
| `README.md` | Project overview and setup guide |
| `.gitignore` | Git exclusion rules |
