# DNS Configuration for kvrretailprivatelimited.online

## Status
✅ Domain purchased: kvrretailprivatelimited.online (Namecheap)
✅ CNAME file created in GitHub repo
⏳ DNS records need to be added manually

## Required DNS Records (Add in Namecheap Advanced DNS)

### For GitHub Pages:
1. **Delete existing parking records** (CNAME and URL Redirect)

2. **Add 4 A Records** (all with Host = "@"):
   - @ → 185.199.108.153
   - @ → 185.199.109.153
   - @ → 185.199.110.153
   - @ → 185.199.111.153

3. **Add CNAME Record**:
   - www → amanmoltbot.github.io

## Quick Instructions:
1. Go to: https://ap.www.namecheap.com/Domains/DomainControlPanel/kvrretailprivatelimited.online/advancedns
2. Remove the 2 existing parking records (Click Remove for each)
3. Click "Add New Record" 5 times to add the records above
4. Click "Save All Changes"

## DNS Propagation
- May take 10-30 minutes for changes to propagate
- Test with: `nslookup kvrretailprivatelimited.online`
- Website will be live at: https://kvrretailprivatelimited.online (and www subdomain)

## Current Status
- Repo: https://github.com/amanmoltbot/kvrretail
- GitHub Pages: https://amanmoltbot.github.io/kvrretail/
- Custom domain configured via CNAME file ✅
