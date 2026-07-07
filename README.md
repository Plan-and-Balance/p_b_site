# Plan & Balance Website

One-page static website for Plan & Balance, built with plain HTML and CSS for GitHub Pages hosting.

## Files

- `index.html`
- `styles.css`
- `README.md`

## Local Preview

Open `index.html` in a browser, or run a simple local server from this folder:

```bash
py -m http.server 8000
```

Then visit `http://localhost:8000`.

## Publish on GitHub Pages

1. Push this folder to a GitHub repository.
2. In GitHub, open **Settings > Pages**.
3. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
4. Select your publishing branch (commonly `main`) and folder (`/root`), then save.
5. Wait for Pages to publish the site.

## Custom Domain (workwithpnb.com)

1. In **Settings > Pages**, set **Custom domain** to `workwithpnb.com` and save.
2. In your DNS provider, create/update records:
	- `A` records for `workwithpnb.com` pointing to GitHub Pages IPs.
	- `CNAME` record for `www` pointing to your GitHub Pages hostname (`<username>.github.io`).
3. In DNS, ensure old conflicting records are removed.
4. Back in GitHub Pages settings, enable **Enforce HTTPS** once available.

## Notes

- This site uses no frameworks, build tools, or external CSS libraries.
- Keep content updates inside `index.html` and style updates inside `styles.css`.
