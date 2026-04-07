# DKTrenchBot v2 Audit Page — Access Instructions

## 🔐 Password-Protected Audit Page

**URL:** https://domx1816-dev.github.io/dktrenchbot-audit/

**Password:** `dkt2026audit`

---

## How It Works

1. Share the URL with auditors
2. They enter the password to access the full audit documentation
3. Once authenticated, the session stays active until they close the browser tab
4. The password gate prevents casual browsing and search engine indexing

---

## Security Notes

⚠️ **This is client-side JavaScript protection**, not military-grade security:
- Prevents casual/unauthorized browsing ✅
- Stops search engines from indexing ✅
- Not suitable for highly sensitive data (password is visible in page source) ✅ Good enough for audit purposes

For true private hosting, you'd need:
- GitHub Pro account ($4/month) for private repos with Pages
- Or a VPS with HTTP auth (nginx basic auth)
- Or Cloudflare Access (paid feature)

---

## Current Setup

- **Repo:** Public (required for free GitHub Pages)
- **Protection:** JavaScript password gate
- **Accessibility:** Anyone with the password can view
- **SEO:** Blocked from search engines by password gate

---

## To Change the Password

Edit `/home/agent/workspace/dktrenchbot-audit/index.html`, find this line:
```javascript
const ACCESS_PASSWORD = 'dkt2026audit';
```

Change `'dkt2026audit'` to your new password, then:
```bash
cd /home/agent/workspace/dktrenchbot-audit
git add -A && git commit -m "Update access password" && git push origin main
```

Pages will rebuild in ~60 seconds.

---

## Quick Test

Visit the URL and enter: `dkt2026audit`

You should see the full audit documentation with wallet addresses, strategy details, and performance metrics.
