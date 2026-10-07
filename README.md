# SyncFlow Group website

Static site (no build step): `index.html` + `assets/`.

## Deploy on GitHub Pages
1. Create a repo and push this folder's contents to the `main` branch (files at the repo root).
2. Repo **Settings → Pages → Build and deployment**: Source = *Deploy from a branch*, Branch = `main`, folder = `/ (root)`.
3. Site goes live at `https://<user>.github.io/<repo>/` within a minute or two.

## Custom domain (e.g. www.syncflow.group)
- Add a `CNAME` file at the root containing just the domain, or set it under Settings → Pages.
- DNS: `www` CNAME → `<user>.github.io`. For the apex domain use GitHub's A records (see GitHub docs).
- Tick **Enforce HTTPS** once the certificate is issued.

## Things to update
- Contact email / website are placeholders (`hello@syncflow.group`) in `index.html`.
- The contact form opens the visitor's email app (`mailto:`). For a real form, use Formspree or similar.
- For social previews (WhatsApp/LinkedIn), set `og:image` to an absolute URL after deploying.
