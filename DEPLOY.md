# Making this site public (GitHub Pages)

Your site will be available at **https://xinyan-wang-stat.github.io** once you complete these steps.

## 1. Push the repo to GitHub

If the repo is not on GitHub yet:

```bash
git remote add origin https://github.com/xinyan-wang-stat/xinyan-wang-stat.github.io.git
git push -u origin master
```

(Use `main` instead of `master` if that is your default branch.)

## 2. Enable GitHub Actions

1. On GitHub, open your repo: **https://github.com/xinyan-wang-stat/xinyan-wang-stat.github.io**
2. Go to **Settings → Actions → General**
3. Under **Workflow permissions**, select **Read and write permissions**
4. Click **Save**

## 3. Set the GitHub Pages source

1. In the same repo, go to **Settings → Pages**
2. Under **Build and deployment**:
   - **Source**: Deploy from a branch
   - **Branch**: `gh-pages` (or the branch your workflow deploys to) and **/ (root)**
   - Click **Save**

The deploy workflow builds the site into the `public` folder and pushes it to the `gh-pages` branch. GitHub Pages will serve the site from that branch.

## 4. Trigger a deploy

- **Option A:** Push a commit to `master` or `main`. The workflow runs automatically.
- **Option B:** Go to **Actions → deploy → Run workflow** and run it manually.

Wait for the workflow to finish (green check in the Actions tab). The site will be live at **https://xinyan-wang-stat.github.io** (it can take a few minutes the first time).

## Troubleshooting

- **404 or “There isn’t a GitHub Pages site here”**  
  Confirm **Settings → Pages** uses branch `gh-pages` and root. Wait 1–2 minutes after the first deploy.

- **Workflow fails**  
  Open **Actions**, click the failed run, and check the error. Common fixes: ensure **Workflow permissions** are **Read and write**, and that the repo has both `master`/`main` (source) and `gh-pages` (deploy) branches after a successful run.

- **Site builds but looks wrong**  
  In `_config.yml`, `url` should be `https://xinyan-wang-stat.github.io` and `baseurl` should be empty for a user site.
