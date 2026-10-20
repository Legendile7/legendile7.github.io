# diveshgupta.com

Astro site deployed to GitHub Pages.

## Run locally
    npm install
    npm run dev

## Deploy
1. Push this folder to a GitHub repo on the `main` branch.
2. In the repo: Settings, Pages, Source: GitHub Actions.
3. Add a custom domain of diveshgupta.com there too, then at your registrar point
   A records to GitHub Pages' IPs (185.199.108.153, .109.153, .110.153, .111.153)
   and a CNAME for www to Legendile7.github.io. public/CNAME already holds the domain.
4. Every push to main rebuilds and deploys via .github/workflows/deploy.yml.

## Editing
- Pages: src/pages/*.astro. Work entries are the `groups` array in work.astro.
- Resume: replace public/Divesh_Gupta_Resume.pdf.
- Styles, nav, footer, and the heading decode effect: src/layouts/Base.astro.
- Landing sphere: the script at the bottom of src/pages/index.astro.
