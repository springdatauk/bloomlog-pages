# BloomLog — public pages (Apple App Review)

Static **Privacy Policy** and **Support** pages for [BloomLog](https://github.com/springdatauk), hosted on **GitHub Pages**.

Support email: **hello@springdata.uk**

## Publish on GitHub (springdatauk)

1. **Create a new public repository** on GitHub under the `springdatauk` org, for example:
   - `bloomlog-pages` (recommended), or  
   - `bloomlog`

2. **Push this folder’s contents** as the repo root (include the `docs` folder and this `README.md`):

   ```bash
   cd bloomlog-pages
   git init
   git add .
   git commit -m "Add BloomLog privacy and support pages for GitHub Pages"
   git branch -M main
   git remote add origin https://github.com/springdatauk/bloomlog-pages.git
   git push -u origin main
   ```

3. **Enable GitHub Pages**
   - Repo → **Settings** → **Pages**
   - **Build and deployment** → Source: **Deploy from a branch**
   - Branch: **main** · Folder: **/docs** → Save

4. After a minute or two, the site will be live at:

   `https://springdatauk.github.io/bloomlog-pages/`

   (Replace `bloomlog-pages` with your actual repo name if different.)

## URLs for App Store Connect

Use these in **App Information** (and Privacy if required):

| Field | URL (example repo `bloomlog-pages`) |
|--------|-------------------------------------|
| **Privacy Policy URL** | `https://springdatauk.github.io/bloomlog-pages/privacy.html` |
| **Support URL** | `https://springdatauk.github.io/bloomlog-pages/support.html` |

If you use a custom domain for GitHub Pages later, replace the host but keep the paths `/privacy.html` and `/support.html`.

## Local preview

Open `docs/index.html` in a browser, or from this directory:

```bash
cd docs && python3 -m http.server 8080
```

Then visit `http://localhost:8080`.

## Files

- `docs/index.html` — landing with links
- `docs/privacy.html` — privacy policy
- `docs/support.html` — support & FAQ
- `docs/css/site.css` — shared styles

Content reflects BloomLog as a **local-only** iOS app (SwiftData on device, optional Pro via **StoreKit** / Apple IAP, no in-app analytics SDKs). Review and adjust if the product changes.
