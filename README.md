# GazetteView

> Search and explore all statutory forms from the Occupational Safety, Health and Working Conditions (Central) Rules, 2026.

A single-file web app — no backend, no build step.

## Features
- Upload up to 4 Gazette PDFs **or** paste extracted text
- Auto-parses every `FORM-I … FORM-XXVII` pattern
- Searchable form index with rule references
- AI Q&A via OpenRouter (free models, no credit card)

## Getting a free OpenRouter key

1. Go to [openrouter.ai/keys](https://openrouter.ai/keys)
2. Sign up (GitHub login works)
3. Create a key — free tier has no credit card requirement
4. Paste it into the app via the **Set API Key** button

## Deploying

### Netlify (easiest — drag & drop)
1. Go to [app.netlify.com](https://app.netlify.com)
2. Drag the entire `GazetteView/` folder onto the deploy zone
3. Done — you get a `*.netlify.app` URL instantly

### Cloudflare Pages
1. Push this repo to GitHub
2. Connect at [pages.cloudflare.com](https://pages.cloudflare.com)
3. Set **build command** to *(empty)* and **output directory** to `/`
4. Deploy → get a `*.pages.dev` URL (custom domain optional)

### GitHub Pages
```bash
git init && git add . && git commit -m "init"
git remote add origin https://github.com/YOUR_USER/gazette-view.git
git push -u origin main
```
Then in Settings → Pages → Source: `main` branch, `/ (root)`.
The app will be live at `https://YOUR_USER.github.io/gazette-view/gazette_form_lookup.html`

## Local use
Just open `gazette_form_lookup.html` in any modern browser. No server needed.
