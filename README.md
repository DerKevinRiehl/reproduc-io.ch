# Reproduc-io website

Static landing page for `reproduc-io.com`, designed for GitHub Pages hosting.

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
7. In the Pages custom domain field, enter `reproduc-io.com`.
8. Save. GitHub will publish the site.
9. In your DNS provider, point `reproduc-io.com` to GitHub Pages.

## DNS setup for custom domain

For the apex domain `reproduc-io.com`, create `A` records pointing to GitHub Pages:

- `185.199.108.153`
- `185.199.109.153`
- `185.199.110.153`
- `185.199.111.153`

Optional but recommended: also create `AAAA` records:

- `2606:50c0:8000::153`
- `2606:50c0:8001::153`
- `2606:50c0:8002::153`
- `2606:50c0:8003::153`

For `www.reproduc-io.com`, create a `CNAME` record pointing to:

- `kriehl.github.io`

Replace `kriehl` if your GitHub username is different.

## Recommended domain verification

GitHub recommends verifying the domain before or during setup to reduce takeover risk.

1. In GitHub, open your account `Settings` -> `Pages`.
2. Add `reproduc-io.com` as a verified domain.
3. GitHub will show a TXT record name and value.
4. Add that TXT record in your DNS provider and keep it there permanently.
5. Return to GitHub and click `Verify`.

## Local preview

Open `index.html` directly in a browser, or serve the folder with any static file server.
