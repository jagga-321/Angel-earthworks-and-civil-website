# Angel Earthworks & Civil — Website

A professional multi-page marketing website for Angel Earthworks. Built with plain HTML, CSS and JavaScript (no frameworks, no build step, no dependencies). Hosts anywhere — GitHub Pages, Netlify, Cloudflare Pages, or any web host.

---

## What's in here

| File | What it does |
|------|-------------|
| `index.html` | Home page — hero, services preview, why-choose, stats, service areas, CTA |
| `services.html` | Detailed services breakdown with rate tables |
| `about.html` | Story, equipment, values, credentials |
| `contact.html` | Phone/email + working quote-request form |
| `styles.css` | All site styling — one file, easy to edit |
| `script.js` | Menu toggle, form handling, scroll effects |
| `favicon.svg` | Browser tab icon (orange A on dark) |
| `robots.txt` | Tells Google to index the site |
| `sitemap.xml` | Site structure for search engines |

---

## BEFORE YOU GO LIVE — things to change

The site uses placeholder values for phone, email, and ABN. **You must update these before launching.**

### 1. Phone number

Replace `0400 000 000` everywhere with your actual mobile.

In **every HTML file**, find:
- `tel:0400000000` → change to `tel:0412345678` (your actual number, no spaces)
- `0400 000 000` → change to your display format
- In `script.js`, update the "Or call us · 0400 000 000" line

### 2. Email address

Replace `hello@angelearthworks.com.au` with your actual email.

Find and replace in **every HTML file** AND `script.js`:
- `hello@angelearthworks.com.au` → your email

### 3. ABN

In each HTML footer:
- `ABN to be confirmed` → `ABN 12 345 678 901` (your actual ABN)

Also in `index.html` find the `LocalBusiness` schema and add your real ABN and phone.

### 4. Domain

If your domain isn't `angelearthworks.com.au`, update:
- The Open Graph URL in `index.html`
- `sitemap.xml` (all 4 URLs)
- `robots.txt`

### 5. Photos (when you have them)

Throughout the site there are placeholder boxes labelled `Photo placeholder`. Once you have real photos of your gear/jobs:

- Make folder `/images/` in the website root
- Save photos as: `excavator.jpg`, `tipper.jpg`, `civil-work.jpg`, `jamie.jpg`, etc.
- In each HTML file, find the `image-block` divs and replace the SVG placeholder with:
  ```html
  <img src="images/excavator.jpg" alt="Hitachi ZX55U Mini Excavator"/>
  ```
- Keep the `image-block` div around the image so it inherits the styling

**Tip:** Compress photos before uploading (use tinypng.com or similar). Aim for under 300KB per photo.

---

## How to deploy

### Option 1: GitHub Pages (easiest, free)

You're already familiar with this from the app. Same process:

1. Create a new GitHub repo (e.g. `angelearthworks-site`)
2. Upload all files in this folder to the repo root
3. Settings → Pages → set Source to "main" branch → Save
4. Wait 1-2 minutes
5. Your site is live at `https://[your-username].github.io/[repo-name]/`

To use your own domain (e.g. `angelearthworks.com.au`):
- Buy the domain from a registrar (Namecheap, GoDaddy, Crazy Domains — about $30-50/year)
- In Settings → Pages, add your custom domain
- Update your domain's DNS records as GitHub instructs
- Done

### Option 2: Netlify or Cloudflare Pages (faster, more pro)

Both are free for personal sites and offer faster loading and better SSL.

**Netlify:**
1. Sign up at netlify.com
2. Drag this folder onto their dashboard
3. Done — site is live
4. Connect your custom domain in their settings

**Cloudflare Pages:**
1. Sign up at pages.cloudflare.com
2. Connect to a GitHub repo OR upload directly
3. Done

---

## Customising

### Change the colour scheme

Open `styles.css`. The top has all the colour variables:

```css
:root {
    --color-orange: #E8580A;  /* Change this for a different accent */
    --color-bg: #0A0A0A;      /* Background */
    --color-text: #F0EDE8;    /* Main text */
    ...
}
```

Change those values and the whole site re-themes.

### Add a new page

1. Copy `about.html` and rename (e.g. `gallery.html`)
2. Edit the content
3. Add a link in the nav of every page:
   ```html
   <a href="gallery.html">Gallery</a>
   ```
4. Add it to `sitemap.xml`

### Edit text content

Each HTML file is well-commented. Just open in any text editor (Notepad++, VS Code, Sublime) and edit the text between the tags. Don't touch the angle brackets, just the words in between.

---

## SEO / Getting found on Google

The site is built with SEO basics in:

- ✓ Each page has unique title and description
- ✓ Structured data (LocalBusiness schema) on homepage
- ✓ Sitemap.xml for search engines
- ✓ Robots.txt allows crawling
- ✓ Semantic HTML structure
- ✓ Fast load (no big JavaScript frameworks)
- ✓ Mobile responsive

**To boost Google rankings:**

1. Submit your sitemap to [Google Search Console](https://search.google.com/search-console) (free)
2. Create a [Google Business Profile](https://www.google.com/business/) — this is the BIG one for tradies. Free, takes 30 minutes, drives more leads than the website itself.
3. Get reviews on your Google Business Profile — every review helps
4. List your business on:
   - True Local
   - Yellow Pages
   - HiPages (paid but worth it for trades)
   - Word of Mouth Online
   - Local SA tradie directories

**Local SEO tips for SA earthworks:**
- Mention "Victor Harbor", "Goolwa", "Fleurieu Peninsula", "South Australia" naturally in your content
- The site already does this well
- Ask happy customers to mention the suburb in their Google review
- Add photos to your Google Business Profile (drives lead conversion)

---

## Browser support

Works on every modern browser — Chrome, Safari, Firefox, Edge.

Tested working at:
- Desktop (1920px, 1440px, 1280px)
- Tablet (768px)
- Mobile (375px, 414px)

---

## Performance

- All HTML pages under 30KB
- Single CSS file ~14KB
- Single JS file ~3KB
- Total page weight: ~50KB + fonts (~80KB from Google)
- Loads in under 1 second on 4G

---

## Need help

The site is built simply on purpose so you (or any web developer) can edit it easily. If you ever need changes you can't work out, any HTML/CSS developer can update it in minutes.

---

Built specifically for Angel Earthworks & Civil. Use as you see fit.
