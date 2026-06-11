# 🌐 Connect Custom Domain to Vercel - Step by Step

## Quick Overview
You need to tell your domain to point to Vercel's servers. This happens in 2 places:
1. **Vercel Dashboard** - Add the domain
2. **Domain Registrar** - Add DNS records

---

## Part 1: Add Domain in Vercel

### Step 1: Go to Your Project
1. Visit: https://vercel.com/dashboard
2. Click on **snf-improvements-v2** project
3. Click **Settings** (top navigation)
4. Click **Domains** (left sidebar)

### Step 2: Add Your Domain
1. You'll see "Add Domain" button
2. Type in your domain:
   - `snfimprovements.com` (root domain)
   - OR `www.snfimprovements.com` (www version)
   - OR both (recommended!)
3. Click **Add**

### Step 3: Vercel Shows You What to Do
After adding, Vercel will display DNS records you need to add. **Keep this page open!**

---

## Part 2: Add DNS Records at Your Domain Registrar

### Where is your domain registered?
Common registrars:
- GoDaddy → godaddy.com
- Namecheap → namecheap.com  
- Google Domains → domains.google.com
- Cloudflare → cloudflare.com
- Others → wherever you bought the domain

### Step 1: Log Into Your Registrar
Go to the website where you bought the domain and log in.

### Step 2: Find DNS Settings
Look for one of these:
- "DNS Management"
- "DNS Settings"  
- "Manage DNS"
- "Domain Settings"
- "Name Servers"

### Step 3: Add the Records Vercel Gave You

Vercel will tell you to add one of these:

#### Option A: A Record (for root domain like snfimprovements.com)
```
Type: A
Name: @ (or leave blank)
Value: 76.76.21.21
TTL: Automatic (or 3600)
```

#### Option B: CNAME Record (for www.snfimprovements.com)
```
Type: CNAME  
Name: www
Value: cname.vercel-dns.com
TTL: Automatic (or 3600)
```

### Step 4: Save Changes
Click "Save" or "Add Record" or "Update"

---

## Part 3: Wait & Verify

### How Long?
- DNS changes take **24-48 hours** to fully propagate
- But usually works in **1-2 hours**
- Sometimes works in **5-10 minutes**!

### Check if it's Working
1. Go back to Vercel → Domains page
2. Look for a ✅ checkmark next to your domain
3. Click "Refresh" if it's been a while
4. Try visiting your domain in a browser

### Troubleshooting
If it's not working after 2 hours:
1. Double-check the DNS records match exactly what Vercel showed
2. Make sure there are no old/conflicting records
3. Try clearing your browser cache (Ctrl+Shift+Delete)
4. Try visiting in incognito/private mode
5. Ask me for help!

---

## Common Domain Registrar Instructions

### GoDaddy
1. Log in → My Products
2. Find your domain → Click DNS
3. Scroll to Records section
4. Click "Add" 
5. Enter the record details
6. Save

### Namecheap  
1. Log in → Domain List
2. Click "Manage" next to your domain
3. Go to "Advanced DNS" tab
4. Click "Add New Record"
5. Enter the record details  
6. Save

### Google Domains
1. Log in → My Domains
2. Click on your domain
3. Go to "DNS" section
4. Scroll to "Custom resource records"
5. Add the record
6. Save

### Cloudflare
1. Log in → Select your domain
2. Go to DNS section
3. Click "Add record"
4. Enter the record details
5. Make sure proxy is OFF (gray cloud, not orange)
6. Save

---

## What if Client Doesn't Have a Domain Yet?

### Option 1: Buy One (Recommended)
**Where to buy:**
- Namecheap (cheap, easy) - ~$10-15/year
- GoDaddy (popular) - ~$15-20/year  
- Google Domains - ~$12/year
- Cloudflare (cheapest) - ~$8-10/year

**What domain to get:**
- snfimprovements.com
- snfimprovements.ca (if in Canada)
- snfrenovations.com
- gosnf.com

### Option 2: Use Vercel's Free Domain (Temporary)
Just use the current link:
https://snf-improvements-v2.vercel.app/

It works perfectly fine! Can always add custom domain later.

---

## SSL Certificate (HTTPS)

**Good news:** Vercel automatically provides FREE SSL certificate!
- Your site will be https:// (secure)
- No extra setup needed
- Automatically renews
- Takes effect within minutes of domain being connected

---

## Need Help?

1. **Send me a screenshot** of what Vercel is telling you to add
2. **Tell me where the domain is registered** (GoDaddy, Namecheap, etc.)
3. **I'll walk you through it** step by step

Or just say: *"Help me connect [domain name] on [registrar]"*

Example: "Help me connect snfimprovements.com on GoDaddy"
