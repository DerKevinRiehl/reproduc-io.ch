# Reproduc-io website

Static landing page for `reproduc-io.ch`, designed for GitHub Pages hosting.

## Files

- `index.html` contains the page structure and marketing copy.
- `styles.css` contains the visual design and responsive layout.
- `script.js` adds scroll reveal animation.
- `CNAME` configures the custom domain for GitHub Pages.
- `.nojekyll` disables Jekyll processing on GitHub Pages.

## Publish on GitHub Pages

1. Create a new GitHub repository and upload these files.
2. Connect this local folder to the repo:
   `git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git`
3. Push the site:
   `git add .`
   `git commit -m "Initial Reproduc-io site"`
   `git push -u origin main`
4. In GitHub, open `Settings` -> `Pages`.
5. Under `Build and deployment`, choose `Deploy from a branch`.
6. Select your `main` branch and the `/ (root)` folder.
7. Save. GitHub will publish the site.
8. In your DNS provider, point `reproduc-io.ch` to GitHub Pages.

## DNS setup for custom domain

For the apex domain `reproduc-io.ch`, create `A` records pointing to GitHub Pages:

- `185.199.108.153`
- `185.199.109.153`
- `185.199.110.153`
- `185.199.111.153`

For `www.reproduc-io.ch`, create a `CNAME` record pointing to:

- `kriehl.github.io`

Replace `kriehl` if your GitHub username is different.

## Local preview

Open `index.html` directly in a browser, or serve the folder with any static file server.
