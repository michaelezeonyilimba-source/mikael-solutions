# mikael.solutions

Personal portfolio and company website for **Michael Ezeonyilimba** — web developer, IT strategist, SaaS builder, and founder of Phguru Integrated Services. Based in Port Harcourt, Rivers State, Nigeria.

## Live Site
🌐 [www.mikael.solutions](https://www.mikael.solutions)

---

## About This Project

A production-ready, single-file SPA (Single Page Application) built with pure vanilla HTML, CSS, and JavaScript — no frameworks, no build tools, no dependencies. Six fully routed pages served from one `index.html` file, deployed on Netlify.

---

## Pages

| Page | Description |
|------|-------------|
| **Home** | Hero, skills overview, projects preview, full experience timeline |
| **Field Work** | Full project portfolio with category filter |
| **Phguru Group** | Company page — Phguru Integrated Services (SMEDAN · SUIN59491788) |
| **About** | Bio, animated skill bars, facts grid, social links |
| **Contact** | Two-column layout with working Netlify Forms integration |
| **Insights** | Live blog powered by Hashnode CMS via GraphQL API |

---

## Tech Stack

- **Frontend** — Vanilla HTML5, CSS3, JavaScript (ES5-compatible)
- **Hosting** — Netlify (free tier)
- **Forms** — Netlify Forms (no backend required)
- **Blog CMS** — Hashnode GraphQL API (headless)
- **Structured Data** — Schema.org JSON-LD
- **Fonts** — Syne, Cormorant Garamond, JetBrains Mono (Google Fonts)

---

## Features

- **SPA routing** — all 6 pages in one HTML file, zero page reloads
- **Mobile-responsive** — hamburger nav drawer, fully responsive grid layouts
- **Scroll reveal animations** — staggered entrance effects on all sections
- **Animated skill bars** — triggered on scroll into view
- **Project filter** — filter Field Work by Web & Apps, IT & Systems, Community & Events, Education
- **Live blog** — fetches posts from Hashnode API; falls back to 6 SEO-ready sample posts
- **Post modal** — reads full articles in-page without leaving the site
- **Blog category filters** — Web Dev, Marketing, Business, AI, Nigeria Tech
- **Netlify Forms** — working contact form with name, email, service, budget, message fields
- **Full SEO** — Open Graph, Twitter Card, canonical URL, meta description
- **Schema.org JSON-LD** — Person, Organization, WebSite, ProfessionalService entities
- **AI search ready** — structured data targets Perplexity, ChatGPT Browse, Gemini citations

---

## Projects Featured

| Project | Type | Status |
|---------|------|--------|
| Ova-Sabi | Multi-tenant SaaS inventory & expiry management | 🟢 Live |
| Rivulet Solutions Ltd | Corporate brand website | 🟢 Live |
| FastFact Services | Marketing services website | 🟢 Live |
| Pyale Workhub | IT lead, CRM, GTM, Merchant Center, React dashboard | 🟢 Live |
| TechBarr Digital Academy | AI & automation training curriculum | Ongoing |
| 2025 Imo State Economic Summit | Head of Implementation, Sub Planning Committee | Completed |
| Youngsters Magazine 2024 | Lead Publisher — YCSN CKC Section | Completed |
| Law Firm Website | Figma design to HTML/CSS deployment | Delivered |

---

## File Structure

```
mikael-solutions/
├── index.html          # Entire website — all 6 pages, CSS, and JS
├── DEPLOYMENT-GUIDE.md # Step-by-step deployment and Hashnode setup
├── README.md           # This file
└── sitemap.xml         # For Google Search Console (create after deployment)
```

---

## Blog Setup (Hashnode)

The blog is pre-wired to Hashnode's GraphQL API. To connect your real posts:

1. Create an account at [hashnode.com](https://hashnode.com)
2. Open `index.html` and find:
   ```js
   var HN_USER = 'phguru';
   ```
3. Replace `phguru` with your actual Hashnode username
4. Redeploy — your live posts appear automatically

Until connected, the blog displays 6 SEO-optimised sample articles.

---

## Deployment

See [`DEPLOYMENT-GUIDE.md`](./DEPLOYMENT-GUIDE.md) for the full step-by-step process covering:

- Netlify drag-and-drop vs GitHub-connected deploy
- Custom domain (mikael.solutions) DNS configuration
- Free SSL setup via Netlify
- Hashnode webhook for auto-rebuild on new posts
- Google Search Console submission
- sitemap.xml creation
- Google Business Profile setup

---

## Company

**Phguru Integrated Services**
SMEDAN Registered · SUIN59491788
Port Harcourt, Rivers State, Nigeria

**Subsidiaries:**
- Phguru Biz Solutions — print, design, document handling, errands, research
- Mikael Solutions — web development, SaaS platforms, IT consulting, smart business systems

---

## Contact

| Channel | Link |
|---------|------|
| Email | michaelezeonyilimba@gmail.com |
| LinkedIn | [linkedin.com/in/michaelezeonyilimba](https://linkedin.com/in/michaelezeonyilimba) |
| Twitter/X | [@ph_guru1](https://x.com/ph_guru1) |
| Instagram | [@michaelxhanson](https://instagram.com/michaelxhanson) |

---

*Built with intent · Phguru Integrated Services · Port Harcourt, Nigeria · 2026*
