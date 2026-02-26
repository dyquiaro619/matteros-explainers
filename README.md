# MatterOS Explainer Site

Static HTML site — ready for one-click Vercel deployment.

## Files

| File | Page |
|------|------|
| `index.html` | Home / Overview |
| `policy-whiplash.html` | Policy Whiplash Explainer |
| `command-bridge.html` | Partner Command Bridge Explainer |
| `signal-authority.html` | Signal Authority Explainer |
| `nav.css` | Shared navigation styles |
| `vercel.json` | Vercel config (clean URLs, security headers) |

## Deploy to Vercel (3 steps)

### Option A — Drag & Drop (Fastest, no account needed*)
1. Go to [vercel.com](https://vercel.com) and sign up / log in (free)
2. From your dashboard click **"Add New → Project"**
3. Drag the entire `matteros-site` folder onto the upload area
4. Click **Deploy** — your site will be live in ~30 seconds

### Option B — GitHub (Recommended for ongoing updates)
1. Create a new GitHub repo (public or private)
2. Push the contents of `matteros-site/` to the repo root
3. In Vercel: **Add New → Project → Import Git Repository**
4. Select the repo → click **Deploy**
5. Every future `git push` will auto-redeploy

### Option C — Vercel CLI
```bash
npm i -g vercel
cd matteros-site
vercel
```
Follow the prompts — first deploy creates the project, subsequent runs update it.

## Custom Domain
After deploying, go to your Vercel project → **Settings → Domains** → add your domain (e.g. `explainers.matteros.com`). Vercel handles SSL automatically.

## URLs after deployment
| Route | Page |
|-------|------|
| `yourdomain.com` | Overview |
| `yourdomain.com/policy-whiplash` | Policy Whiplash |
| `yourdomain.com/command-bridge` | Command Bridge |
| `yourdomain.com/signal-authority` | Signal Authority |

*`cleanUrls: true` in vercel.json removes the `.html` extension automatically.*
