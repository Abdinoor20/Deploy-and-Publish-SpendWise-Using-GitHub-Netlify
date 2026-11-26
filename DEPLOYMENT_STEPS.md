# Your deployment checklist (not part of the submission)

You can delete this file before pushing, or keep it.

## 1. Test locally
Open `index.html` in your browser (or use the VS Code Live Server extension). Click through all pages, add a few transactions.

## 2. Push to GitHub
1. On github.com click **New repository**, name it `spendwise`, choose **Public**, do NOT add a README (you already have one).
2. In the project folder:
   ```
   git init
   git add .
   git commit -m "Initial commit: SpendWise"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/spendwise.git
   git push -u origin main
   ```

## 3. Deploy on Netlify
1. Log in at netlify.com (use "Log in with GitHub").
2. **Add new site > Import an existing project > GitHub**, pick `spendwise`.
3. Build command: leave empty. Publish directory: `.` (already set in `netlify.toml`).
4. Click **Deploy**.

## 4. Custom site name
**Site configuration > General > Site details > Change site name** (for example `spendwise-yourname`). Your URL becomes `https://spendwise-yourname.netlify.app`.

## 5. Continuous deployment test
Edit the footer in all pages from `SpendWise v1.0` to `SpendWise v1.1` (or change the heading text), then:
```
git add .
git commit -m "Update footer version to v1.1"
git push
```
Watch **Deploys** in Netlify, then refresh your live site and confirm the change.

## 6. Final README
Put your real GitHub link and Netlify URL in `README.md`, rewrite the Challenges and Lessons sections in your own words, commit, push, and submit only the GitHub link in the LMS.
