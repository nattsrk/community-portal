# Community Portal — Demo

A modern, responsive demo of the **Community Portal** — a community website covering
members, jobs, matrimony, an e‑store, services, resources, about, contact and registration.

🔗 **Live demo:** https://nattsrk.github.io/community-portal/

> **Demo only.** This is a front‑end demo. There is no backend or database — the
> registration and contact forms validate input and show a success message but do not
> store any data. Some avatars use [placehold.co](https://placehold.co) placeholders;
> product and hero photos are from [Unsplash](https://unsplash.com).

## Features

- **Modern UI** — clean design system built with Tailwind 3, the Inter typeface,
  glassmorphism sticky navbar, gradient hero bands, elevated hover cards and a dark footer.
- **Theme toggle** — switch the whole site between two palettes from the navbar:
  - **Warm Sand** (default) — taupe hero bands with bronze accents.
  - **Navy & Gold** — deep‑navy hero bands with gold accents.
  The choice is remembered per visitor (localStorage) and applied before paint (no flash).
- **Community hero** — the homepage uses a community photo with a theme‑tinted overlay.
- **Localized content** — Indian member/team names and prices in **₹ (INR)**.
- **Fully responsive** — mobile menu, fluid grids, works from phone to desktop.
- **Zero build step** — plain HTML + CDN assets; just open or serve the folder.

## Pages

| Page | File | Notes |
|------|------|-------|
| Home | `index.html` | Hero (community photo), features, stats, events, CTA |
| About | `about.html` | Mission/vision, values, leadership team, impact stats |
| Members | `members.html` | Member directory cards |
| Jobs | `jobs.html` | Community job board with search/filters |
| Matrimony | `matrimony.html` | Profiles + ₹ membership plans |
| Store | `store.html` | E‑store product grid (real product photos, ₹ prices) |
| Services | `services.html` | Service groups + plan cards |
| Resources | `links.html` | Resource/link directory |
| Contact | `contact.html` | Contact form + info panel |
| Register | `register.html` | Registration form (client‑side validation, demo only) |
| Complete | `complete.html` | Post‑registration welcome / story page |

> `navbar.html` is a shared nav fragment and `elements.html` is an unused reference template.

## Tech

- Plain HTML + [Tailwind CSS 3](https://tailwindcss.com) (Play CDN)
- [Inter](https://fonts.google.com/specimen/Inter) font + [Font Awesome 6](https://fontawesome.com) (CDN)
- Theming via CSS custom properties switched by a `data-theme` attribute
- No build step, no dependencies

## Run locally

Any static file server works, e.g.:

```bash
python3 -m http.server 8099
# then open http://localhost:8099
```

## Deployment

Published via **GitHub Pages** from the `gh-pages` branch (root).
`main` holds the source of truth and is kept in sync.

```
main        → source of truth
gh-pages    → what GitHub Pages serves (live)
```
