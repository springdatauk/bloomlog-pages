# BloomLog — public pages (Apple App Review)

Static **Privacy Policy**, **Support**, and **Terms of Use (EULA)** pages for BloomLog, hosted on **GitHub Pages**.

- **Repository:** [github.com/springdatauk/bloomlog-pages](https://github.com/springdatauk/bloomlog-pages)  
- **Live site:** [springdatauk.github.io/bloomlog-pages](https://springdatauk.github.io/bloomlog-pages/)

Support email: **hello@springdata.uk**

## Already published

This repo is wired to **GitHub Pages** (source: **main** → **/docs**). To update the site after editing files:

```bash
cd bloomlog-pages
git add -A && git commit -m "Update pages" && git push
```

## URLs for App Store Connect

Use these in **App Information** (and Privacy if required):

| Field | URL (example repo `bloomlog-pages`) |
|--------|-------------------------------------|
| **Privacy Policy URL** | `https://springdatauk.github.io/bloomlog-pages/privacy.html` |
| **Support URL** | `https://springdatauk.github.io/bloomlog-pages/support.html` |
| **Terms (EULA)** | `https://springdatauk.github.io/bloomlog-pages/terms.html` (links to Apple’s standard EULA) |

If you use a custom domain for GitHub Pages later, replace the host but keep the paths.

**App Store:** If you use Apple’s **standard** EULA, also put this link in the **App Description**:  
`https://www.apple.com/legal/internet-services/itunes/dev/stdeula/`

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
- `docs/terms.html` — Terms of Use; points to Apple’s standard App Store EULA
- `docs/css/site.css` — shared styles

Content reflects BloomLog as a **local-only** iOS app (SwiftData on device, optional Pro via **StoreKit** / Apple IAP, no in-app analytics SDKs). Review and adjust if the product changes.
