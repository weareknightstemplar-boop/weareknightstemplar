# 30-Day Warrior Challenge - Website Setup Guide
## Complete Sales Funnel Integration

---

## 📁 What You Have

This folder contains your complete sales funnel:

| File | Purpose |
|------|---------|
| `index.html` | Main landing page with email capture + payment |
| `30_day_warrior_challenge_cover.jpg` | Product cover image |
| `7-Prayers-for-the-Modern-Warrior-FREE.pdf` | Lead magnet (free offer) |
| `30-Day-Warrior-Challenge-DELUXE.pdf` | Paid product ($27) |
| `EMAILS_READY_TO_PASTE.txt` | 7-email sequence for ConvertKit |

---

## 🚀 How to Upload to GitHub & Vercel

### Step 1: Prepare Your Files

1. **Open this folder** on your computer
2. **Select ALL files** in this folder (Ctrl+A on Windows, Cmd+A on Mac)
3. **Compress/ZIP them** (right-click → "Compress" or "Send to ZIP")

### Step 2: Upload to GitHub

1. Go to **github.com** and sign in
2. Find your repository (e.g., `weareknightstemplar-website`)
3. Click **"Add file"** → **"Upload files"**
4. **Drag & drop** your ZIP file OR click "choose your files"
5. Scroll down, add a commit message: `Updated landing page with email capture`
6. Click **"Commit changes"**

### Step 3: Vercel Auto-Deploys

✅ **Vercel automatically deploys** when you push to GitHub

1. Go to your Vercel dashboard
2. Your site will show "Building..." then "Ready"
3. Your live URL updates automatically

---

## 💳 How to Connect Payment Portal (Gumroad)

### Option A: Simple Link (Recommended)

1. Go to **gumroad.com** → Your Products
2. Click on **"30-Day Warrior Challenge"**
3. Click **"Share"** tab
4. Copy your product URL (looks like: `https://gumroad.com/l/XXXXX`)
5. Open `index.html` in a text editor
6. Find this line (around line 975):
   ```html
   <a href="https://gumroad.com/l/30-day-warrior-challenge" class="cta-button">
   ```
7. **Replace** the URL with your actual Gumroad link
8. Save and re-upload to GitHub

### Option B: Embedded Gumroad Button (More Professional)

Add this script to your `<head>` section for overlay checkout:

```html
<script src="https://gumroad.com/js/gumroad.js"></script>
```

Then your button becomes:
```html
<a href="https://gumroad.com/l/YOUR-LINK" class="gumroad-button">Buy Now</a>
```

---

## 📧 How the Email Funnel Works

### Current Flow:

```
Visitor Lands on Page
       ↓
[Hero Section] - Sees $27 offer
       ↓
[Email Section] - Offered 7 Free Prayers
       ↓
Enters Email → ConvertKit captures it
       ↓
Auto-sent: 7 Prayers PDF (you set this up in ConvertKit)
       ↓
7-Day Email Sequence begins...
       ↓
Day 4: Pitches 30-Day Challenge ($27)
       ↓
Day 7: Membership offer
```

### Setting Up the Email Sequence in ConvertKit:

1. Go to **ConvertKit** → **Automations**
2. Create **"New Automation"**
3. Trigger: **"Subscribes to form"** → Select your "7 Prayers" form
4. Add emails from `EMAILS_READY_TO_PASTE.txt`
5. Set delays between emails (recommended: 1 day apart)

---

## ⚙️ Customization Checklist

### Must Update:

- [ ] **Gumroad Link** in index.html (line ~975)
- [ ] **ConvertKit Form ID** (already done - your form: 54448a7d37)
- [ ] **Email Sequence** in ConvertKit (paste from EMAILS_READY_TO_PASTE.txt)
- [ ] **Upload PDFs** to ConvertKit for auto-delivery

### Optional:

- [ ] Add Google Analytics tracking
- [ ] Connect custom domain on Vercel
- [ ] Add Facebook Pixel for retargeting

---

## 🔗 Important Links

| Platform | URL | Purpose |
|----------|-----|---------|
| Your Website | `https://weareknightstemplar.vercel.app` | Live landing page |
| GitHub Repo | `github.com/YOURNAME/weareknightstemplar` | Edit files here |
| ConvertKit | `convertkit.com` | Email automation |
| Gumroad | `gumroad.com` | Payment processing |
| Vercel | `vercel.com` | Hosting dashboard |

---

## 🆘 Troubleshooting

### "Page not updating after GitHub upload"
- Vercel takes 30-60 seconds to rebuild
- Check Vercel dashboard for build errors
- Hard refresh: Ctrl+Shift+R (Windows) or Cmd+Shift+R (Mac)

### "Emails not being captured"
- Verify ConvertKit form ID: `54448a7d37`
- Check form is set to "inline" format in ConvertKit
- Test by submitting your own email

### "Payment button not working"
- Make sure Gumroad link is complete (includes `https://`)
- Test the link directly in browser first
- Check Gumroad product is published (not draft)

---

## 📊 Next Steps to Maximize Revenue

1. **Set up abandoned cart emails** in Gumroad
2. **Add testimonials** as you get them
3. **Create urgency** with limited-time bonuses
4. **A/B test headlines** using Vercel split testing
5. **Retargeting ads** on Facebook/Instagram

---

**Deus Vult!** 🛡️⚔️

Questions? The funnel is live and ready—just update your Gumroad link and you're in business.
