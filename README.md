# Peeely — React + Tailwind CSS rebuild

React 19 · Vite · Tailwind CSS v4 · Framer Motion · Lenis (smooth scroll) · React Router · Lucide

```bash
npm install
npm run dev      # http://localhost:5173
npm run build    # production build in /dist
```

## Structure

```
src/
  assets/        images, logos, icons, avatars … (+ index.js registry: import { images, logos } from '../assets')
  components/
    layout/      Navbar, Footer, StickyPromo, Layout, SmoothScroll (Lenis + hash scrolling)
    ui/          Button, Marquee, Reveal, SectionHeading, RatingBadge, HashLink
  data/content.js  ALL copy, prices, FAQ, team, reviews — edit text here
  sections/      Hero, TrustedCases, ValueProp, Comparison, Features, Showcase,
                 HowItWorks, Reviews, Pricing, Team, CaseStudies, Faq
  pages/         Home, CaseStudy, Contact, Legal, SimplePages (BrandBrief, ThankYou)
  index.css      Tailwind theme tokens (colors, fonts, keyframes)
```

Design tokens live in `src/index.css` (`--color-lime`, `--color-forest`, `--color-navy`, …).

## Content notes

- FAQ answers, legal pages and case-study copy for Vynta / Lunara / Elevatearc are written placeholders —
  the original export only contained the questions / Nuvia's full text. Replace them in `data/content.js`
  and `pages/Legal.jsx`.
