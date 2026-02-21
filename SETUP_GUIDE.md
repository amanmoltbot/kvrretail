# KVR Retail - Complete Setup Guide

## ✅ Completed

### 1. Website Created & Deployed
- **URL**: https://amanmoltbot.github.io/kvrretail/
- **GitHub Repo**: https://github.com/amanmoltbot/kvrretail
- **Status**: Live and accessible
- Clean, professional company information site with all required details

## 🔄 Next Steps

### 2. Domain Registration (Manual Step Required)

**Recommended Domain**: `kvrretailprivatelimited.online`

**Price**: ₹88.88/year (~$1.10 USD) - Well under $3 budget

**Alternative Options** (same price):
- kvrretailprivatelimited.store
- kvrretailprivatelimited.site

**To Purchase on Namecheap**:
1. Go to: https://www.namecheap.com/domains/registration/results/?domain=kvrretailprivatelimited
2. Click "Add to cart" for `.online` domain
3. Complete checkout
4. Total cost: ₹88.88/year

**After Purchase**:
- Update nameservers to Cloudflare (for free email routing)
- Or keep Namecheap DNS and add MX records manually

### 3. Email Setup Options

Once domain is purchased, choose ONE of these free options:

#### Option A: Cloudflare Email Routing (Recommended - Simplest)

**Requirements**: 
- Free Cloudflare account
- Domain nameservers pointed to Cloudflare

**Steps**:
1. Sign up at https://dash.cloudflare.com
2. Add your domain (kvrretailprivatelimited.online)
3. Update nameservers at Namecheap to Cloudflare's NS
4. Go to Email → Email Routing
5. Create catch-all or specific address: info@kvrretailprivatelimited.online
6. Forward to: amanmoltbot@gmail.com (or any existing email)
7. Verify email forwarding
8. Done! You can now receive emails

**Pros**: 
- Completely free
- No storage limits (it's just forwarding)
- Can send from Gmail using "Send mail as"
- Very reliable

#### Option B: Zoho Mail Free Tier

**Requirements**:
- Access to domain DNS settings

**Steps**:
1. Sign up at https://www.zoho.com/mail/
2. Verify domain ownership via TXT record
3. Add MX records to domain DNS:
   ```
   Priority 10: mx.zoho.in
   Priority 20: mx2.zoho.in
   ```
4. Add SPF record:
   ```
   v=spf1 include:zoho.in ~all
   ```
5. Create email account: info@kvrretailprivatelimited.online
6. Access via: https://mail.zoho.com

**Pros**:
- Real mailbox (can send and receive)
- 5GB storage
- Professional email interface

**Cons**:
- More setup steps
- Limited to 5 users on free tier

#### Option C: ImprovMX (Forwarding Only)

**Requirements**:
- Access to domain DNS settings

**Steps**:
1. Go to https://improvmx.com/
2. Add domain: kvrretailprivatelimited.online
3. Add MX records:
   ```
   Priority 10: mx1.improvmx.com
   Priority 20: mx2.improvmx.com
   ```
4. Set up forwarding: *@kvrretailprivatelimited.online → amanmoltbot@gmail.com
5. Verify in ImprovMX dashboard

**Pros**:
- Very simple
- Free forever
- Catch-all forwarding

**Cons**:
- Forwarding only (can't send from domain email directly)

### 4. Connect Website to Domain

After domain purchase, update GitHub Pages:

```bash
cd /Users/molt/Projects/kvrretail
echo "kvrretailprivatelimited.online" > CNAME
git add CNAME
git commit -m "Add custom domain"
git push
```

Then in Namecheap DNS, add:
```
A Record: @ → 185.199.108.153
A Record: @ → 185.199.109.153
A Record: @ → 185.199.110.153
A Record: @ → 185.199.111.153
CNAME: www → amanmoltbot.github.io
```

Or if using Cloudflare, add same records there.

## Summary

**Total Cost**: ~$1.10/year for domain

**What You Get**:
1. Professional website: kvrretailprivatelimited.online
2. Professional email: info@kvrretailprivatelimited.online
3. Ability to receive verification codes
4. Full company information online

**Time to Complete** (after domain purchase): ~15-30 minutes
