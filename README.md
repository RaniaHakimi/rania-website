# Rania Hakimi — personal website

A single-page personal site. Plain HTML/CSS, no build step, no dependencies.

## Structure

```
.
├── index.html    # the entire site (edit this)
├── .nojekyll     # tells GitHub Pages to serve files as-is
├── .gitignore
└── README.md
```

## Editing

Everything lives in `index.html`. Search for the `<!-- EDIT -->` comments to find the
spots to change:

- **Links** — replace `you@example.com`, the GitHub URL, and the LinkedIn URL.
- **Projects** — swap the three `Project one/two/three` entries for real work (or delete any you don't need).
- **About / Focus / tagline** — reword to sound like you.

To preview locally, just open `index.html` in a browser (double-click it).

## Deploy with GitHub Pages (free)

1. Create a new repository on GitHub and push this folder to it:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO.git
   git push -u origin main
   ```
2. On GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, pick `main` / `/ (root)`, and **Save**.
3. Your site goes live at `https://YOUR-USERNAME.github.io/YOUR-REPO/` within a minute or two.

> Tip: if you name the repo `YOUR-USERNAME.github.io`, it publishes at the root
> `https://YOUR-USERNAME.github.io/` instead of a subpath.

## Connect your custom domain

1. In **Settings → Pages → Custom domain**, enter your domain and Save. GitHub creates a
   `CNAME` file in the repo automatically.
2. At your domain registrar's DNS settings, add:
   - Four **A records** for the root (`@`) pointing to GitHub Pages:
     `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - One **CNAME record** for `www` pointing to `YOUR-USERNAME.github.io`
3. Back in **Settings → Pages**, tick **Enforce HTTPS** once the certificate is issued
   (can take a little while after DNS propagates).

## License

Personal project — feel free to add a license file if you want one.
