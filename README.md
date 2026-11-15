# meni – opening soon

Single-page "opening soon" site for **meni**, a shop for graphic clothing, framed art, books and accessories.

- One self-contained `index.html` (inline CSS and JS, Jost via Google Fonts)
- Light and dark mode aware, responsive, respects `prefers-reduced-motion`
- Light/dark theme toggle (remembers the choice)
- Interactive 3D-style totem: tilts with the pointer, layers shift for depth, the eye follows the cursor, tap a shape to recolour and spin it
- Motion: drifting colour orbs, rotating rings, scrolling ticker
- Email signup form with validation

## Run locally

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
```

## Signups by email

Submissions go to `kabare1k@gmail.com` through [FormSubmit](https://formsubmit.co) (no account needed).

**One-time activation:** after deploying, open the live site, submit your own email once, then click the activation link FormSubmit sends to kabare1k@gmail.com. Until then, signups show an error. It does not work from a `file://` page, only from a hosted URL.

Change `FORM_ENDPOINT` in `index.html` to use another service.

## Deploy with GitHub Pages

A workflow in `.github/workflows/pages.yml` deploys on every push to `main`.
In the repo go to **Settings → Pages → Source → GitHub Actions**.
