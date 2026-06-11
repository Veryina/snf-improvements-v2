# SNF Improvements V2 - Complete Guide

## ✅ What's Been Updated

### Contact Information Changed:
- **Name:** Sivan Gourgees  
- **Phone:** (416) 702-3303 (updated everywhere)
- **Email:** snfimprovement@gmail.com (updated everywhere)

### New Features Added:
- ✅ Instagram feed section (ready for photos)
- ✅ All contact info updated throughout site
- ✅ Mobile responsive Instagram grid

---

## 📸 How to Add Instagram Feed

The site is ready for an Instagram feed. You have **3 options**:

### Option 1: Manual Photos (Simplest - DO THIS)
Upload 6-9 project photos and I'll hardcode them into the Instagram section. Just send me the images!

### Option 2: Instagram Embed Widget (Free, No Coding)
Use a service like:
- **EmbedSocial** (embedsocial.com)
- **SnapWidget** (snapwidget.com)
- **Elfsight** (elfsight.com)

Steps:
1. Sign up for free account
2. Connect Instagram
3. Customize widget appearance
4. Copy the embed code
5. Send me the code and I'll add it

### Option 3: Instagram Basic Display API (Advanced)
Requires Facebook Developer account and app setup. Not recommended unless you want automatic feed updates.

---

## 🌐 How to Connect Custom Domain on Vercel

### Step 1: Access Domain Settings
1. Go to https://vercel.com/dashboard
2. Find the **snf-improvements-v2** project
3. Click on it
4. Go to **Settings** → **Domains**

### Step 2: Add Your Domain
1. Click **"Add Domain"**
2. Enter your domain (e.g., `snfimprovements.com` or `www.snfimprovements.com`)
3. Click **"Add"**

### Step 3: Configure DNS Records

Vercel will show you what DNS records to add. You'll need to add these at your domain registrar (GoDaddy, Namecheap, etc.)

#### If using root domain (snfimprovements.com):
Add **A Record**:
```
Type: A
Name: @
Value: 76.76.21.21
```

#### If using www subdomain (www.snfimprovements.com):
Add **CNAME Record**:
```
Type: CNAME
Name: www
Value: cname.vercel-dns.com
```

#### For both (recommended):
Add both records above, then in Vercel set one to redirect to the other.

### Step 4: Where to Add DNS Records

**At Your Domain Registrar:**
1. Log into where you bought the domain (GoDaddy, Namecheap, etc.)
2. Find "DNS Management" or "DNS Settings"
3. Add the records Vercel showed you
4. Save changes

**DNS propagation takes 24-48 hours** (but usually works in 1-2 hours)

### Step 5: Verify in Vercel
- Go back to Vercel → Domains
- You should see a checkmark when it's working
- If not, click "Refresh" or wait a bit longer

---

## 📱 How to Upload Project Photos

### For Instagram Section:
Send me 6-9 project photos and I'll add them to the site.

**Photo Requirements:**
- Square format (1:1 ratio) works best
- High quality (at least 1000x1000px)
- Show your best work!
- Good lighting

### For Gallery Section (if you want to replace Unsplash placeholders):
Same as above, but rectangular photos work too.

---

## 🚀 Deploy Updated Site

Once you send me photos or we make more changes:

```bash
cd /root/.openclaw/workspace/snf-improvements-v2
git add .
git commit -m "Updated contact info and added Instagram section"
git push origin main
```

Vercel will auto-deploy in ~30 seconds!

---

## 📋 Current Project Structure

```
snf-improvements-v2/
├── index.html          ← Main website (all updated!)
├── .vercel/            ← Vercel config
│   └── project.json
└── COMPLETE-GUIDE.md   ← This file
```

---

## ✅ Checklist

- [x] Contact info updated (Sivan Gourgees, new phone/email)
- [x] Instagram section added
- [ ] Upload project photos (need from client)
- [ ] Add Instagram feed (Option 1, 2, or 3 above)
- [ ] Connect custom domain (if client has one)
- [ ] Test on mobile
- [ ] Deploy final version

---

## 🆘 Need Help?

**To deploy now:**
Just say "deploy snf v2" and I'll push it live.

**To add photos:**
Send them to me and say "add these photos to SNF instagram section"

**To connect domain:**
Tell me the domain name and where it's registered, I'll walk you through it.

**Current Live URLs:**
- V2 (current): https://snf-improvements-v2.vercel.app/
- V1 (old): https://snf-improvements.vercel.app/
- V3 (experimental): https://snf-improvements-v3.vercel.app/
