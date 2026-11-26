# SpendWise

## Project Description

SpendWise is a simple personal expense tracker. You can record income and expenses, see your current balance, review spending by category for the month, and search, filter, export (CSV) or delete past transactions. All data is saved in the visitor's browser (local storage), so no server or database is needed. This project was built as a static website and published to the internet using GitHub and Netlify.

## Technologies Used

- HTML5
- CSS3 (responsive layout, no frameworks)
- JavaScript (vanilla, browser local storage)
- Git and GitHub (version control and source hosting)
- Netlify (hosting and continuous deployment)

## GitHub Repository Information

- Repository: https://github.com/YOUR-USERNAME/spendwise
- Visibility: Public
- Main branch: `main`

### Project structure

```
spendwise/
├── index.html          Dashboard (add transactions, summary, categories)
├── transactions.html   Search, filter, export and delete transactions
├── about.html          About page
├── 404.html            Custom "page not found" page
├── css/style.css       Styles
├── js/app.js           Shared helpers (storage, formatting)
├── js/dashboard.js     Dashboard logic
├── js/transactions.js  Transactions page logic
├── assets/             Logo and favicon
├── netlify.toml        Netlify settings
└── README.md
```

## Live Website

**Live Netlify URL:** https://YOUR-SITE-NAME.netlify.app

## Deployment Process Summary

1. Checked that all files were organised correctly, that `index.html` sits in the project root, and that every link, stylesheet, script and image uses a relative path.
2. Created a public repository on GitHub and pushed the project with Git (`git init`, `git add .`, `git commit`, `git remote add origin ...`, `git push -u origin main`).
3. Logged in to Netlify, chose **Add new site > Import an existing project**, connected GitHub and selected the SpendWise repository. Build command: none. Publish directory: the repository root (`.`).
4. Deployed the site, then changed the default random subdomain to a meaningful one under **Site configuration > Change site name**.
5. Tested continuous deployment: changed the footer version from `v1.0` to `v1.1`, committed and pushed to GitHub, and confirmed Netlify automatically rebuilt and the live site showed the change.
6. Tested the live site: all three pages and the 404 page load, the CSS, JavaScript and images load, transactions can be added, filtered, exported and deleted, and the site works on a phone-sized screen.

## Challenges Encountered During Deployment

> Replace this section with your own real experience. Examples of common issues:

- Broken CSS or JavaScript links because of wrong file paths or different letter case (Netlify's servers are case-sensitive, e.g. `Style.css` vs `style.css`).
- `index.html` not being in the root folder, which caused a "Page not found" error.
- Git authentication when pushing to GitHub for the first time.
- Waiting for the deploy to finish and forgetting to hard refresh (Ctrl + Shift + R) when checking an update.

## Lessons Learned

> Replace with your own words. Examples:

- Deployment is much easier when the project structure and relative paths are correct from the start.
- Continuous deployment means every push to GitHub updates the live site, so changes should be tested locally first.
- Netlify's deploy log is the first place to look when something goes wrong.
- A clear README makes a project easier for others to understand and review.
