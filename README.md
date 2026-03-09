# Agentic LX — AI Reception System for WhatsApp Businesses

> **Your business never sleeps. Neither does your AI.**

A single-file landing page for Agentic LX — fully self-contained HTML/CSS/JS.

---

## 🗂 File Structure

```
/
├── index.html   ← Full website (HTML + CSS + JS, all inline)
├── CNAME        ← Custom domain (edit before deploying)
└── README.md    ← This file
```

---

## 🚀 Deploy to GitHub Pages

### Step 1 — Create a GitHub repository

1. Go to [github.com/new](https://github.com/new)
2. Name it anything (e.g. `agenticlx-site`)
3. Set it to **Public**
4. Click **Create repository**

### Step 2 — Push the code

Open a terminal in the project folder and run:

```bash
git init
git add .
git commit -m "Initial deploy — Agentic LX landing page"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO.git
git push -u origin main
```

> Replace `YOUR-USERNAME` and `YOUR-REPO` with your actual GitHub username and repository name.

### Step 3 — Enable GitHub Pages

1. In your repository, go to **Settings → Pages**
2. Under **Source**, select:
   - Branch: `main`
   - Folder: `/ (root)`
3. Click **Save**
4. GitHub will show a URL like `https://your-username.github.io/your-repo/`

Your site will be live in ~60 seconds. ✅

---

## 🌐 Connect a Custom Domain

### Step 1 — Edit the CNAME file

Open `CNAME` and replace `YOUR-DOMAIN.COM` with your actual domain:

```
agenticlx.com
```

Commit and push the change:

```bash
git add CNAME
git commit -m "Set custom domain"
git push
```

### Step 2 — Add a DNS record with your registrar

Log in to your domain registrar (GoDaddy, Namecheap, Cloudflare, etc.) and add:

| Type  | Name  | Value                            | TTL  |
|-------|-------|----------------------------------|------|
| CNAME | `www` | `YOUR-USERNAME.github.io`        | Auto |
| A     | `@`   | `185.199.108.153`                | Auto |
| A     | `@`   | `185.199.109.153`                | Auto |
| A     | `@`   | `185.199.110.153`                | Auto |
| A     | `@`   | `185.199.111.153`                | Auto |

> The four `A` records point the root domain (`@`) directly to GitHub Pages IPs.

### Step 3 — Configure in GitHub Settings

1. Go to **Settings → Pages → Custom domain**
2. Enter your domain (e.g. `agenticlx.com`) and click **Save**
3. Wait for DNS propagation (usually 5–30 minutes)

### SSL / HTTPS

GitHub Pages provisions a **free Let's Encrypt SSL certificate** automatically once:
- DNS has propagated
- The custom domain is verified

Check the **"Enforce HTTPS"** checkbox in Settings → Pages once it appears.

---

## 🔄 Updating the Site

Make edits to `index.html`, then push:

```bash
git add index.html
git commit -m "Update: [describe change]"
git push
```

GitHub Pages redeploys automatically within ~30 seconds.

---

## 📞 Support

Built by [Agentic LX](mailto:hello@agenticlx.com) · WhatsApp: [+91 99999 99999](https://wa.me/919999999999)
