# Nandani Khandelwal — Premium Portfolio

A single-file, dependency-free portfolio site with a dark glassmorphism design
(blue → cyan → purple gradients), built for GitHub Pages.

## Files to upload to your repo (all in one folder, at the root)
- `index.html` — the entire site (HTML + CSS + JS, no build step)
- `Nandani_Khandelwal_Resume.pdf` — used by the "Download Resume" button

## Deploy on GitHub Pages
1. Create a repo, e.g. `nandani-portfolio`.
2. Upload both files above to the repo root.
3. Settings → Pages → Source: **Deploy from a branch** → branch `main`, folder `/ (root)` → Save.
4. Live in ~1–2 minutes at `https://<username>.github.io/<repo-name>/`.

## What changed in this redesign (UI/UX only — content unchanged)
- Dark glass theme (#0B1120) with blue/cyan/purple gradients, Space Grotesk + Inter typography, 8px spacing scale.
- Full-screen animated hero: floating gradient blobs, a light canvas particle field, a typing effect that cycles Data Analyst / Power BI Developer / SQL Enthusiast / Python Learner, gradient name text, and CTA + social buttons.
- Sticky glass navbar with scroll-based active-section highlighting, animated mobile hamburger menu, scroll progress bar, and a cursor glow effect (desktop only).
- About section: animated-border profile card, 4 stat counters that count up on scroll, and an animated timeline for education.
- Skills grouped into Data Analytics / Programming / Visualization / Soft Skills, with animated progress bars and hover-glow chips.
- Projects as glass cards with an illustrated chart thumbnail, tech badges, feature lists, tilt-on-hover, and a working technology filter (All / Power BI / Tableau / Excel).
- Experience shown as an animated vertical timeline; Certifications as hover-lift badge cards.
- Contact section with a floating-label form (opens a pre-filled email — this is a static site with no backend, so there's no server to send from), contact-info cards, and an embedded map centered on Jaipur.
- Footer with social icons, credit line, and a back-to-top button.
- Respects `prefers-reduced-motion`, uses visible focus states, and all effects are plain CSS/JS (no external animation library needed) so the page loads instantly with zero dependencies beyond Google Fonts.

## Two honest calls I made
1. Your resume didn't include a "problem solving questions solved" figure, so I used **months of industry experience (4)** for the 4th stat card instead of inventing a number.
2. Neither project has a public live demo link, so the "Live Demo" button is shown but disabled/greyed rather than pointing somewhere fake — swap in a real link any time by editing the `<a>`/`<span>` in the project card.

## Editing
Everything lives in `index.html`. Content sections are commented (`<!-- ============ SECTION ============ -->`) so you can find About/Skills/Projects/etc. quickly. Colors and spacing are defined once at the top of the `<style>` block under `:root` — change those to retheme the whole site.
