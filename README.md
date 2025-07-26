# CDN via GitHub Pages

This repository can be used as a free CDN using GitHub Pages. Upload files to the `images` or `scripts` folder and access them via:

```
https://<username>.github.io/<repo>/images/<file>
https://<username>.github.io/<repo>/scripts/<file>
```

A minimal Decap CMS is available under `/admin/` for uploading images or creating Markdown content without using git.

## Enable GitHub Pages
1. Open the repository on GitHub.
2. Go to **Settings → Pages**.
3. Under **Source**, select the **`main`** branch and save.

GitHub Pages will provide URLs in the form `https://<username>.github.io/<repo>/`.

### Custom domain
To use a custom domain (e.g. `cdn.mydomain.com`), create a **CNAME** record pointing `cdn.mydomain.com` to `<username>.github.io`. Then add the same domain in the GitHub Pages custom domain field.

## SPA fallback
The included `404.html` redirects unknown paths to the site root so it can be used to host single page applications.
