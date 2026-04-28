# Portfolio for GitHub Pages

This project is ready to be published as a static site on GitHub Pages.

## What is already prepared

- Relative links between the main page and project pages
- Static HTML/CSS/JS structure that works on GitHub Pages
- `.nojekyll` file to prevent GitHub Pages from applying Jekyll processing

## Recommended repository contents

Upload these items to the repository root:

- `index.html`
- `projects/`
- `assets/`
- `Картинки для проектов портфолио/`

Large export folders like `surge-dist/`, `surge-fast-dist/`, `cloudflare-pages-dist/` are not required for GitHub Pages.

## Publish on GitHub Pages

1. Create a GitHub repository.
2. Upload the site files to the repository root.
3. Push to the `main` branch.
4. Open `Settings -> Pages`.
5. In `Build and deployment`, choose:
   - `Source`: `Deploy from a branch`
   - `Branch`: `main`
   - `Folder`: `/ (root)`
6. Save the settings.

After deployment:

- If the repository is named `username.github.io`, the site will open at:
  - `https://username.github.io/`
- If the repository has any other name, the site will open at:
  - `https://username.github.io/repository-name/`

## Custom domain

GitHub Pages supports a custom domain.

To connect it:

1. Open `Settings -> Pages`.
2. In `Custom domain`, enter your domain.
3. Add the required DNS records at your domain registrar.
4. Enable HTTPS in GitHub Pages after DNS starts resolving correctly.

Typical DNS setup:

- For a subdomain like `portfolio.example.com`:
  - create a `CNAME` record pointing to `username.github.io`
- For an apex/root domain like `example.com`:
  - use the DNS records GitHub Pages shows in the settings panel

Official docs:

- [GitHub Pages Quickstart](https://docs.github.com/en/pages/quickstart)
- [Custom domain setup](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)
