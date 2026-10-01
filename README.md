<h1 align="center">Hi 👋, I'm Udayraj Sahu</h1>
<h3 align="center">"React.js Developer | Frontend Enthusiast | Exploring 3D Web Experiences"</h3>

<p align="left"> <img src="https://komarev.com/ghpvc/?username=udayraj-sahu&label=Profile%20views&color=0e75b6&style=flat" alt="udayraj-sahu" /> </p>

- 🌱 I’m currently learning **Three.js**

- 👨‍💻 All of my projects are available at [udayraj-portfolio-beta.vercel.app](https://udayraj-portfolio-beta.vercel.app/)

- 📫 How to reach me **udayrajsahu123@gmail.com**

<h3 align="left">Connect with me:</h3>
<p align="left">
<a href="https://www.linkedin.com/in/udayraj-sahu-a20490422/" target="_blank" rel="noopener noreferrer"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="LinkedIn" height="30" width="40" /></a>
<a href="https://www.instagram.com/dev.udayraj/" target="_blank" rel="noopener noreferrer"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/instagram.svg" alt="Instagram" height="30" width="40" /></a>
</p>

<h3 align="left">Languages and Tools:</h3>
<p align="left"> <a href="https://getbootstrap.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-plain-wordmark.svg" alt="bootstrap" width="40" height="40"/> </a> <a href="https://www.cprogramming.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/c/c-original.svg" alt="c" width="40" height="40"/> </a> <a href="https://www.w3schools.com/cpp/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/cplusplus/cplusplus-original.svg" alt="cplusplus" width="40" height="40"/> </a> <a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/> </a> <a href="https://www.w3.org/html/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg" alt="html5" width="40" height="40"/> </a> <a href="https://www.java.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg" alt="java" width="40" height="40"/> </a> <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> </a> <a href="https://www.mongodb.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mongodb/mongodb-original-wordmark.svg" alt="mongodb" width="40" height="40"/> </a> <a href="https://nodejs.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original-wordmark.svg" alt="nodejs" width="40" height="40"/> </a> <a href="https://reactjs.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original.svg" alt="react" width="40" height="40"/> </a> </p>

<p><img align="center" src="https://github-readme-stats.vercel.app/api/top-langs?username=udayraj-sahu&show_icons=true&locale=en&layout=compact" alt="udayraj-sahu" /></p>

---

## About this repository

This repo contains the source for the portfolio site deployed at
[udayraj-portfolio-beta.vercel.app](https://udayraj-portfolio-beta.vercel.app/).

A single-page developer portfolio built as a terminal-inspired interface, with
an interactive terminal, expandable project archive and FAQ accordion.

### Stack

| Layer     | Choice                                                  |
| --------- | ------------------------------------------------------- |
| Build     | Vite 8                                                  |
| UI        | React 19 + TypeScript 5.7                               |
| Styling   | Tailwind CSS v4                                         |
| Animation | GSAP 3 + ScrollTrigger, plus CSS scroll-driven fallback |
| Platform  | Figma Make                                              |

### Running locally

`pnpm` is the intended package manager, but any npm-compatible client works.

```bash
npm install       # or: pnpm install
npm run dev       # Vite dev server, defaults to http://127.0.0.1:8443
npm run build     # type-checks and emits dist/
npm run preview   # serve the production build locally
```

### Project layout

```
src/
  App.tsx                  page composition shell
  components/              shared UI (Nav, Cursor, ProjectRow, TerminalScreen…)
    ui/                    primitives (SectionHeader, Divider, SectionLabel)
  data/                    all content as typed modules (profile, faq, seo, site)
  hooks/                   scroll-linked animation hooks
  lib/anim/                GSAP wrappers, reveals, scramble, view transitions
  sections/                one component per page section
  types.ts                 shared domain types
scripts/
  audit-responsive.mjs     headless overflow / touch-target audit across widths
  probe.mjs                nav-visibility and accordion-expansion behaviour probe
  make-og-image.ps1        regenerates public/og-image.png
```

Content lives in `src/data/profile.ts` — projects, skills and contact links are
edited there, not inside components.

### Responsive and accessibility notes

- Layout is verified from 320px to 1920px. `scripts/audit-responsive.mjs` drives
  the running dev server through the Chrome DevTools Protocol and fails on
  horizontal overflow or touch targets under 44px.
- The custom cursor is mounted only where `(hover: hover) and (pointer: fine)`
  matches, so tap targets keep the native cursor on touch devices.
- All animation respects `prefers-reduced-motion`; the page renders identically,
  just static.
- Accordions animate with `grid-template-rows: 0fr → 1fr` so they expand to their
  content's natural height with no hard-coded `max-height` to clip on mobile.

### Licence

Private / personal project. All rights reserved.
