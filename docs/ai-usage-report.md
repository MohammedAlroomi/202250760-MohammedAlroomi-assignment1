# AI Usage Report

**Assignment:** Assignment 1 – Foundation & AI Integration
**Course:** SWE 363 – Web Development
**Student:** Mohammed Alroomi (202250760)
**Date:** February 2026

---

## Tools Used & Use Cases

I used two AI tools throughout this assignment: **Claude (claude.ai)** and **ChatGPT (OpenAI)**, each serving a distinct role.

### Claude (claude.ai) — Primary Development Tool

Claude was my main tool for code generation, debugging, and documentation. I used it iteratively — describing requirements, reviewing output, asking follow-up questions, and refining before including anything in the project.

- **Code Generation:** Generated the HTML structure, CSS theming system, responsive layout, and all JavaScript features. I broke requests into focused tasks (navbar, hero, projects, etc.) so I could read and understand each piece before moving on.
- **Debugging:** When the hamburger menu wasn't working, I described the issue to Claude and it identified that opening via `file://` protocol can block JavaScript — pointing me to test via a local server or GitHub Pages.
- **Code Review:** After assembling the project, Claude flagged missing `aria-label` attributes on interactive buttons, which I added to improve accessibility.
- **Documentation & Content:** I shared my CV with Claude to help draft the About Me section, project descriptions, and experience entries, which I then reviewed and edited for accuracy.
- **UI/UX Suggestions:** When undecided on the Experience layout, Claude recommended a timeline card design over a plain list, explaining it communicates professional progression more clearly. I agreed and implemented it.

### ChatGPT (OpenAI) — Concept Clarification Tool

I used ChatGPT to understand concepts before implementing them — a "learn first, then build" approach.

- **IntersectionObserver API:** Claude's scroll animation code used this API which I hadn't seen before. ChatGPT explained how it works and why it's more efficient than scroll event listeners, giving me the confidence to include and understand it.
- **CSS Grid vs Flexbox:** ChatGPT clarified when to use each, helping me verify that Claude's layout choices were correct — Grid for two-dimensional sections, Flexbox for one-dimensional flows like the navbar.
- **sessionStorage vs localStorage:** When Claude suggested `localStorage` for the theme preference, ChatGPT explained the difference. I decided `sessionStorage` was sufficient and instructed Claude to update it accordingly.

---

## Benefits & Challenges

**Benefits:**
Using AI significantly accelerated development without bypassing learning. I spent less time on syntax lookup and more time understanding design decisions and testing. Claude introduced me to patterns I wouldn't have found alone — CSS custom properties for theming, `IntersectionObserver` for animations, and organized JavaScript function structure. Using two tools with different strengths also let me cross-check decisions before committing to them.

**Challenges:**
The initial HTML output contained generic placeholders that required multiple follow-up prompts to personalize. Claude also occasionally over-engineered solutions — suggesting a `localStorage` expiry system for the theme toggle — so I had to guide it toward simpler, scope-appropriate alternatives. Not everything worked perfectly out of the box either; the `backdrop-filter` blur effect on the navbar required a `-webkit-` vendor prefix for Safari that Claude had missed, which I discovered through manual browser testing and fixed independently.

---

## Learning Outcomes

- **CSS Custom Properties:** Learned to use them as a full design token system — swapping an entire theme by toggling one class on `<body>`.
- **IntersectionObserver API:** A new and more performant alternative to scroll event listeners for triggering animations, which I'll carry into future projects.
- **Semantic HTML:** Consistently using `<nav>`, `<section>`, `<footer>`, `<label>`, and `<form>` with proper attributes became a natural habit through this project.
- **JavaScript organization:** Structuring features as named, single-responsibility functions called from one `DOMContentLoaded` listener made the code cleaner and easier to debug.
- **Effective AI use:** The biggest lesson was that productive AI use is iterative and specific. Narrow, contextual prompts produce far better results than vague ones — and every output needs to be reviewed, tested, and understood before it becomes your work.

---

## Responsible Use & Modifications

All AI-generated output was treated as a draft. Key modifications I made:

- **Personalization:** Replaced all placeholder content with my real information — projects (ISE291, COE292, ICS321), experience (Okoul, McKinsey EDAD, SAC), and contact details from my CV.
- **Privacy:** Independently decided to remove my GPA and phone number from the public portfolio after Claude pulled them from my CV.
- **Creative additions:** The terminal widget in the Hero section was my own concept — I asked Claude to implement it, but the idea was mine. Font pairing and accent color were also my own aesthetic choices.
- **Simplification:** Removed over-engineered suggestions and replaced them with cleaner alternatives appropriate for the assignment scope.
- **Comments & testing:** All inline code comments were written by me after understanding each function. All responsive and cross-browser testing was performed manually by me.

I can explain every line of code in this project. AI accelerated and informed my work — it did not replace my thinking or learning.