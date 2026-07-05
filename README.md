# Portfolio — Mora Upendhra Chary

A dependency-free personal portfolio built with plain HTML, CSS and
JavaScript. No build tools, no frameworks — open `index.html` in a browser
or deploy the folder as-is.

## Folder structure

```
Portfolio/
├── index.html          Main page (all sections)
├── css/
│   └── style.css       Design tokens, layout, components, animations
├── js/
│   └── script.js        Nav, theme toggle, typing effect, scroll reveal, form
├── images/              SVG placeholders (avatar + 6 project thumbnails)
└── assets/
    └── Upendhra_Chary_Mora_Resume.pdf   Downloadable resume
```

## Customize

- **Profile photo**: replace `images/avatar.svg` with a real photo
  (`.jpg`/`.png`), then update the `src` in the hero's `.avatar-frame` in
  `index.html`.
- **Project thumbnails**: replace `images/project-1.svg` … `project-6.svg`
  with real screenshots (same filenames, or update the `src` attributes).
- **LinkedIn URL**: search `index.html` for `href="#"` next to the LinkedIn
  icons and swap in your profile link.
- **Resume file**: swap `assets/Upendhra_Chary_Mora_Resume.pdf` for an
  updated export whenever your resume changes (keep the same filename, or
  update the two `href` references in `index.html`).
- **Contact form**: the form currently simulates a send in `js/script.js`
  (`initContactForm`). Wire it to a real backend, or a service like
  Formspree / EmailJS, by replacing the `setTimeout` block with a `fetch()`
  call.
- **Google Map**: the `.map-placeholder` block in the Contact section is a
  visual placeholder — swap it for a real `<iframe>` embed from Google Maps.
- **Colors / fonts**: everything is driven by CSS variables at the top of
  `css/style.css` (`:root` and `[data-theme="dark"]`) — change the palette
  or type scale in one place.

## Deploy

This is static, so it's ready to go on:

- **GitHub Pages** — push the folder to a repo and enable Pages on the
  `main` branch (`/` root).
- **Netlify** — drag-and-drop the `Portfolio` folder onto Netlify's deploy
  screen, or connect the repo.
- **Vercel** — import the repo as a static project (no framework preset
  needed).

No build step is required for any of the above.
