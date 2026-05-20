# ReaDax

Static website starter for ReaDax, currently set up for GitHub Pages.

## Local Preview

From this folder:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## GitHub Pages

This repo includes a GitHub Actions workflow at `.github/workflows/pages.yml`
that deploys the static site from the repository root. In GitHub, set the
Pages source to **GitHub Actions**, then set the custom domain to `readax.ai`
in the Pages settings.

The `CNAME` file records `readax.ai` as the intended canonical domain. Change
that file too if you decide to make `readax.info` or `readax.io` primary
instead, especially if you later switch Pages back to branch-based publishing.

## Domains

Canonical setup:

- Use `readax.ai` as the landing page and canonical site.
- Point `www.readax.ai` to the GitHub Pages host so GitHub can redirect it to
  `https://readax.ai`.
- Redirect `readax.info`, `www.readax.info`, `readax.io`, and `www.readax.io`
  to `https://readax.ai` at the registrar, DNS provider, or a redirect-capable
  service such as Cloudflare.
