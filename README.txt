Monte Cafe - Static site copy
Files:
- index.html
- assets/logo.png

How to deploy (pick one):
1) GitHub Pages (easy)
   - Create a GitHub repo. For user pages: name it username.github.io and push these files to the main branch.
   - Or create a normal repo, push and enable Pages in repo Settings (serve from main branch / root).
   - Optional: add a CNAME file with your custom domain.

2) Netlify (drag-and-drop)
   - Drop the zip or the folder into Netlify's 'Sites' -> 'Add new site' -> 'Deploy manually'.
   - Or connect the GitHub repo to Netlify for continuous deploys.

3) Vercel / Cloudflare Pages: connect GitHub repo and follow prompts.

DNS (connect your GoDaddy domain):
- Point the domain to your host following their docs:
  * GitHub Pages: add A records to GitHub's IPs or add CNAME for 'www' to username.github.io (see GitHub Pages docs).
  * Netlify/Vercel: follow the provider's instructions (usually add CNAME for www and set ALIAS/ANAME for root).
- Enable HTTPS via the hosting provider (they provide free TLS automatically).

Notes:
- If your original site had server-side features (forms, databases), you'll need serverless functions or third-party providers.
- Update internal links to be relative (they already are).
