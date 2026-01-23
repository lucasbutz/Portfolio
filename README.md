# Deploying this site

This repository contains a single static page: `index.html`.

Below are simple, copy-paste steps to host it on popular static hosts. Pick one and follow the commands.

Local test
```
# Serve locally on port 8000
python3 -m http.server 8000
# or with Node (if installed)
npx http-server -p 8000
```

Option A — GitHub Pages (recommended if you use GitHub)
- Initialize and push to GitHub:
```
git init
git add .
git commit -m "Initial commit"
# create a repo on GitHub (use the web UI) named e.g. 'portfolio'
git remote add origin git@github.com:<your-username>/portfolio.git
git branch -M main
git push -u origin main
```
- Enable GitHub Pages: go to the repository Settings → Pages and select the `main` branch (root) as the source. The site will be published at `https://<your-username>.github.io/portfolio/`.

Option B — Netlify (drag & drop or CLI)
- Drag & drop: go to https://app.netlify.com/drop and upload the project folder.
- Netlify CLI deploy:
```
npm install -g netlify-cli
netlify login
netlify init    # follow prompts to create new site
netlify deploy --prod --dir=.
```

Option C — Vercel
```
npm i -g vercel
vercel login
vercel            # follow prompts, choose project directory '.'
```

Option D — Cloudflare Pages
- Create a Pages project at https://dash.cloudflare.com/pages and connect to your Git repository (GitHub/GitLab).

Custom domain
- All providers support custom domains. Add your domain in provider settings and update DNS records as instructed by the provider.

Next steps I can do for you
- Initialize a git repo locally and create the first commit.
- Help create a GitHub repo and push (you'll need to authenticate).
- Deploy to Netlify/Vercel if you authorize me (or I can give exact commands for you to run).

Tell me which provider you prefer and whether you want me to initialize git and prepare a push from this machine.
