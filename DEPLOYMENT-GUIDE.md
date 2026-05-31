# mikael.solutions — Deployment Guide
### Michael Ezeonyilimba · Phguru Integrated Services

---

## WHAT YOU HAVE

One file: `mikael-solutions.html`

This is your complete website — 6 pages in one file (Home, Field Work, Phguru Group, About, Contact, Insights/Blog). Rename it `index.html` before deploying.

**Pages included:**
- Home — hero, what I do, projects preview, experience, blog strip, contact CTA
- Field Work — 9 projects with filter by category (Web, IT, Community, Education)
- Phguru Group — company page with both subsidiaries + 9 services
- About — bio, facts, skill bars, social links
- Contact — two-column layout with working Netlify form
- Insights — live blog powered by Hashnode CMS (with 6 sample posts until you connect Hashnode)

**Built with:**
- Pure HTML, CSS, JavaScript — no frameworks, no build tools needed
- Netlify Forms (contact form — works automatically on Netlify)
- Hashnode GraphQL API (blog — optional, see Step 3)
- Schema.org structured data (SEO + AI search engines)
- Full Open Graph / Twitter card meta tags

---

## STEP 1 — DEPLOY TO NETLIFY (10 minutes)

### Option A: Drag and Drop (Easiest)

1. Rename the file from `mikael-solutions.html` to `index.html`
2. Go to **netlify.com** and sign up / log in (free)
3. On your dashboard, look for the box that says **"Drag and drop your site folder here"**
4. Create a folder on your computer called `mikael-solutions`
5. Put `index.html` inside that folder
6. Drag the entire `mikael-solutions` folder into Netlify's drop zone
7. Wait ~15 seconds. Netlify gives you a temporary URL like `random-name.netlify.app`
8. Your site is live!

### Option B: GitHub + Netlify (Better for updates)

1. Create a GitHub account at github.com if you don't have one
2. Create a new repository called `mikael-solutions`
3. Upload `index.html` to the repository (rename it first)
4. In Netlify: New site → Import from Git → Connect GitHub → Select your repo
5. Build settings: leave everything blank (no build command, no publish directory)
6. Click Deploy
7. Every time you update the file and push to GitHub, Netlify auto-deploys

---

## STEP 2 — CONNECT YOUR DOMAIN (mikael.solutions)

After purchasing `mikael.solutions` (see recommended registrars below):

1. In Netlify: Go to your site → **Domain management** → **Add custom domain**
2. Type: `mikael.solutions` → Click Verify → Add domain
3. Netlify shows you **DNS records** to add:
   - Type A: `75.2.60.5`
   - Type CNAME: `www` pointing to `your-site.netlify.app`
4. Log into your domain registrar (Truehost, Fimgohost, DomainKing etc.)
5. Find **DNS settings** or **Name servers**
6. Add the records Netlify shows you
7. Wait 15 minutes to 2 hours for DNS to propagate
8. Your site is live at `www.mikael.solutions`!

**Netlify also gives you FREE SSL (HTTPS) automatically** — no extra setup needed.

### Cheapest Domain Registrars (Pay in Naira):
- **Truehost Nigeria** — truehost.com.ng — ~₦12,000–₦20,000/year for .com
- **Fimgohost** — fimgohost.com — Naira billing, no FX markup, free WHOIS privacy
- **DomainKing** — domainking.ng — accredited .NG registrar

**mikael.solutions** is a premium domain extension. Check:
- Porkbun.com (USD, cheapest for .solutions globally ~$5-12/year)
- Namecheap.com (USD)
- Or use **mikael.com.ng** which is cheaper and signals Nigerian professional

---

## STEP 3 — CONNECT BLOG TO HASHNODE (20 minutes, optional)

The blog currently shows 6 sample articles. To publish real posts:

### 3a. Create Hashnode Account
1. Go to **hashnode.com** → Sign up with Google
2. Choose a username — use **phguru** or **michaelezeonyilimba**
3. Create your publication (your blog)

### 3b. Update the Website
Open `index.html` in any text editor (Notepad, VS Code)  
Find this line near the bottom:
```
var HN_USER = 'phguru';
```
Change `phguru` to your actual Hashnode username  
Save the file and re-upload to Netlify

### 3c. Connect Webhook (Auto-rebuilds)
1. In Netlify: Site settings → **Build hooks** → Add build hook → Name it "Hashnode" → Copy the URL
2. In Hashnode: Publication settings → **Integrations** → Webhooks → Add webhook → Paste Netlify URL
3. Now every post you publish on Hashnode automatically rebuilds your live site!

### Writing Posts That Rank:
Write posts with titles like:
- "Web developer for hire in Port Harcourt Nigeria"
- "How to build a SaaS platform in Nigeria 2026"
- "Best coworking space Port Harcourt"
- "IT consulting services Port Harcourt"
- "How I built my first web app as a Nigerian developer"

Use these **tags** in Hashnode to match the blog filter buttons:
`Web Development`, `Digital Marketing`, `Business`, `AI`, `Nigeria Tech`

---

## STEP 4 — SUBMIT TO GOOGLE (15 minutes)

After your domain is live:

1. Go to **search.google.com/search-console**
2. Add property → Enter `https://www.mikael.solutions`
3. Verify ownership (Netlify DNS method is easiest)
4. Submit your sitemap: `https://www.mikael.solutions/sitemap.xml`  
   *(Note: you'll need to create a sitemap.xml — see below)*
5. Request indexing of your homepage

### Create sitemap.xml
Create a new file called `sitemap.xml` in your folder with this content:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
  <url>
    <loc>https://www.mikael.solutions/</loc>
    <changefreq>weekly</changefreq>
    <priority>1.0</priority>
  </url>
  <url>
    <loc>https://www.mikael.solutions/#work</loc>
    <changefreq>monthly</changefreq>
    <priority>0.9</priority>
  </url>
  <url>
    <loc>https://www.mikael.solutions/#blog</loc>
    <changefreq>weekly</changefreq>
    <priority>0.9</priority>
  </url>
</urlset>
```

Upload this file alongside your `index.html` in the same folder.

---

## STEP 5 — GOOGLE BUSINESS PROFILE

1. Go to **business.google.com**
2. Add your business: **Mikael Solutions** or **Phguru Integrated Services**
3. Category: Web Design Agency / IT Services
4. Location: Port Harcourt, Rivers State, Nigeria
5. Website: `https://www.mikael.solutions`
6. This puts you on Google Maps and boosts local search ranking

---

## CONTACT FORM

The contact form uses **Netlify Forms** — it works automatically when deployed to Netlify.

- Submissions appear in: Netlify dashboard → Your site → **Forms**
- Set up email notifications: Forms → Settings → Email notifications → Add your email
- No backend, no code, no monthly cost — completely free up to 100 submissions/month

---

## UPDATING THE WEBSITE

To update any content (text, add a project, change your bio):

1. Open `index.html` in VS Code or any text editor
2. Use Ctrl+F to search for the text you want to change
3. Edit it
4. Save the file
5. Drag the updated folder to Netlify OR push to GitHub if using Option B

---

## SEO ALREADY BUILT IN

The website already includes:
- **Meta description** — shows in Google search results
- **Open Graph tags** — controls how it looks when shared on LinkedIn/Facebook/Twitter
- **Twitter Card** — preview image and description on Twitter/X
- **Schema.org JSON-LD** — structured data for Person, Organization, WebSite, ProfessionalService
- **Canonical URL** — tells Google the authoritative URL
- **Twitter/X creator tag** — `@ph_guru1`

This is why AI search engines (Perplexity, ChatGPT Browse) will be able to cite you directly.

---

## QUICK REFERENCE

| Item | Value |
|------|-------|
| Your email | michaelezeonyilimba@gmail.com |
| LinkedIn | linkedin.com/in/michaelezeonyilimba |
| Twitter/X | x.com/ph_guru1 |
| Instagram | instagram.com/michaelxhanson |
| SMEDAN Reg | SUIN59491788 |
| Ova-Sabi live | ovasabitracker.netlify.app |
| Rivulet | rivuletsolutions.com |
| FastFact | fastfactservices.com |
| Pyale Workhub | pyaleworkhub.com |

---

*Phguru Integrated Services · mikael.solutions · Port Harcourt, Nigeria*
