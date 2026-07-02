[README.md](https://github.com/user-attachments/files/29616309/README.md)
# AJ's 5 Star Services — Website

A static site (plain HTML/CSS/JS, no build step) with three pages:
- `index.html` — Home
- `government-contracting.html` — Government Contracting
- `contact.html` — Contact

## Deploy to Vercel (no coding required for this part)

**Option A — Drag and drop (fastest):**
1. Go to https://vercel.com and sign up (free)
2. From the dashboard, click **Add New → Project**
3. Choose **"Deploy without Git"** / drag-and-drop upload, and drop this entire `site` folder in
4. Vercel auto-detects it as a static site — click **Deploy**
5. You'll get a live URL immediately (something like `aj5star.vercel.app`)

**Option B — Connect a GitHub repo (better for ongoing edits):**
1. Create a free GitHub account and a new repository
2. Upload this folder's contents to that repository
3. In Vercel, click **Add New → Project → Import Git Repository**, and select it
4. Leave all build settings as default (no framework, no build command needed — it's static)
5. Click **Deploy**

Either way, once deployed you can connect your own domain (e.g. `aj5starservices.com`) under **Project → Settings → Domains** in Vercel, and update your domain's DNS records as instructed there.

## Before you launch — things to finish

- [ ] **Capability Statement PDF** — replace `assets/capability-statement.pdf` (currently a placeholder) with your real one, keeping the same filename so the download buttons keep working
- [ ] **Email / phone** — replace the placeholder `info@aj5starservices.com` and `(000) 000-0000` throughout (found in `index.html`, `government-contracting.html`, `contact.html`)
- [ ] **LinkedIn URL** — update the placeholder link in `contact.html`
- [ ] **Contact form** — this is a static site, so the form needs a form-handling service to actually deliver submissions to your inbox. Easiest option: sign up free at https://formspree.io, create a form, and replace `YOUR_FORM_ID` in `contact.html`'s `<form action="...">` with your real form ID. Takes about 5 minutes.
- [ ] **Government Contracting data** — fill in UEI, CAGE code, SAM registration date, NAICS codes, business classifications, service area, and insurance details (currently marked `[placeholder]` in `government-contracting.html`)
- [ ] **Company legal name** — confirm entity type (LLC/Inc.) in the data sheet

## Making edits later

Every page is plain HTML — open any `.html` file in a text editor (VS Code recommended, free at https://code.visualstudio.com) and edit the text directly between tags. Styling lives in one place: `css/style.css`. Colors and fonts are defined as variables at the very top of that file under `:root`, so changing e.g. the gold accent color everywhere means changing one line.

If you'd rather not hand-edit code going forward, you can always come back and ask for help with specific changes — just describe what you want changed and on which page.

## File structure
```
site/
├── index.html
├── government-contracting.html
├── contact.html
├── css/
│   └── style.css
├── js/
│   └── main.js
├── assets/
│   ├── how-we-work-flow.svg
│   └── capability-statement.pdf   (placeholder — replace with real file)
└── README.md
```
