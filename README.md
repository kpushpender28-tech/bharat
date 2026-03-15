# 🌿 Bharat Vandana Park — Official Tourism Website

A complete, professional static tourism website for Bharat Vandana Park, Dwarka, Delhi — built with pure HTML, CSS, and JavaScript. GitHub Pages compatible. No backend required.

---

## 📁 Project Structure

```
bharat-vandana-park/
│
├── index.html          ← Homepage (Hero, Attractions, Gallery preview, FAQ)
├── about.html          ← About page (History, Design, Timeline)
├── attractions.html    ← All 10 zones in detail
├── gallery.html        ← Photo gallery with filter
├── visiting-info.html  ← Tickets, timings, how to reach, facilities
├── contact.html        ← Contact form, map, department contacts
│
├── css/
│   └── style.css       ← Complete stylesheet (1,000+ lines)
│
├── js/
│   └── script.js       ← Hero slider, FAQ, lightbox, scroll reveal
│
├── images/
│   └── (placeholder — all images load from Unsplash CDN)
│
└── README.md
```

---

## 🚀 How to Deploy on GitHub Pages

### Step 1: Create a GitHub Account
Visit https://github.com and sign up for a free account.

### Step 2: Create a New Repository
1. Click the **"+"** icon → **New repository**
2. Repository name: `bharat-vandana-park` (or any name you like)
3. Set to **Public**
4. Click **Create repository**

### Step 3: Upload Files
**Option A — GitHub Web Interface (Easiest):**
1. Open your new repository
2. Click **"Add file"** → **"Upload files"**
3. Drag and drop the ENTIRE `bharat-vandana-park` folder contents
4. Commit message: `Initial website upload`
5. Click **"Commit changes"**

**Option B — Git Command Line:**
```bash
git init
git add .
git commit -m "Initial commit — Bharat Vandana Park website"
git remote add origin https://github.com/YOUR_USERNAME/bharat-vandana-park.git
git branch -M main
git push -u origin main
```

### Step 4: Enable GitHub Pages
1. Go to your repository → **Settings** tab
2. Scroll to **Pages** in the left sidebar
3. Under **Source**, select **"Deploy from a branch"**
4. Branch: **main** | Folder: **/ (root)**
5. Click **Save**
6. Wait 2–3 minutes

### Step 5: Access Your Website
Your website will be live at:
```
https://YOUR_USERNAME.github.io/bharat-vandana-park/
```

---

## 🌐 How to Connect Your GoDaddy Domain

### Step 1: Set Up Custom Domain in GitHub Pages
1. Repository → **Settings** → **Pages**
2. Under **Custom domain**, type your domain (e.g., `bharatvandanapark.in`)
3. Click **Save**
4. GitHub will create a `CNAME` file in your repository

### Step 2: Configure DNS Records in GoDaddy
1. Log in to **GoDaddy** → **My Products** → **DNS Management**
2. Delete any existing A records pointing to the same domain

**Add these A Records** (GitHub Pages IP addresses):
| Type | Host | Value | TTL |
|------|------|-------|-----|
| A | @ | 185.199.108.153 | 600 |
| A | @ | 185.199.109.153 | 600 |
| A | @ | 185.199.110.153 | 600 |
| A | @ | 185.199.111.153 | 600 |

**Add CNAME Record** (for www):
| Type | Host | Value | TTL |
|------|------|-------|-----|
| CNAME | www | YOUR_USERNAME.github.io | 3600 |

### Step 3: Enable HTTPS
1. Wait 24–48 hours for DNS to propagate
2. GitHub → Settings → Pages → Check **"Enforce HTTPS"**
3. Your site will be live at `https://bharatvandanapark.in`

### Step 4: Verify Domain (Optional but Recommended)
Go to GitHub → Settings → Pages → Verify your domain to prevent domain hijacking.

---

## 🎨 Website Pages Overview

| Page | File | Key Features |
|------|------|-------------|
| Homepage | index.html | Hero slider, Stats counter, Attractions, Mini India band, Gallery preview, FAQ |
| About | about.html | History, Key facts, Design philosophy, Interactive timeline |
| Attractions | attractions.html | All 10 zones, 20 monument chips, Detailed zone descriptions |
| Gallery | gallery.html | 20 photos, 7 category filters, Lightbox viewer |
| Visitor Info | visiting-info.html | Ticket table, Timings, Google Maps embed, Facilities, Rules |
| Contact | contact.html | Contact form, Map, Department contacts, Location info |

---

## ✏️ How to Customize Content

### Change Text Content
Open any `.html` file in a text editor (Notepad, VS Code, etc.) and edit the text directly.

### Change Images
Replace Unsplash URLs with your own images:
```html
<!-- Replace this URL -->
<img src="https://images.unsplash.com/photo-XXXXX?w=600&q=80" alt="Description" />

<!-- With your own image -->
<img src="images/your-photo.jpg" alt="Description" />
```
Put your images in the `/images/` folder.

### Change Colors
Open `css/style.css` and edit the CSS variables at the top:
```css
:root {
  --saffron:    #E65100;  /* ← Change primary orange/saffron color */
  --green-dark: #1B5E20;  /* ← Change primary green color */
  --gold:       #F9A825;  /* ← Change accent gold color */
}
```

### Update Ticket Prices
Open `visiting-info.html` and find the ticket table to update prices.

### Update Contact Information
Open `contact.html` and update phone numbers, email addresses, and address.

### Add/Remove FAQ Items
Open `index.html`, find the `.faq-grid` section, and copy/paste a `.faq-item` block.

---

## ⚡ Performance Features

- All images loaded from Unsplash CDN (fast global delivery)
- CSS animations are hardware-accelerated (transform/opacity only)
- Fonts loaded from Google Fonts CDN
- No external JavaScript libraries required
- Lazy loading on iframes
- Minimal HTTP requests

---

## 🔍 SEO Features

- Semantic HTML5 structure
- Meta title and description on every page
- Canonical URLs
- Open Graph tags
- Schema-ready structure
- Clean URL structure compatible with GitHub Pages

---

## 📱 Browser & Device Support

Tested and compatible with:
- Chrome, Firefox, Safari, Edge (latest versions)
- iOS Safari & Chrome
- Android Chrome
- Screen widths from 320px to 2560px

---

## 📄 Image Credits

All images are sourced from **Unsplash** (unsplash.com) under the Unsplash License, which allows free use for commercial and non-commercial purposes without attribution (though attribution is appreciated).

For copyright-free monument images:
- Wikimedia Commons: commons.wikimedia.org (CC BY-SA)
- PIB India: pib.gov.in (Government open content)

---

## 📞 Support

For questions about the park, contact:
- **DDA Helpline:** 1800-11-0332 (Toll Free)
- **Email:** bvp@dda.gov.in
- **Website:** https://dda.gov.in

---

*Built with ❤️ for Bharat Vandana Park — Delhi Development Authority*
