# Amir Fard portfolio

Ready-to-upload static website. No build tools are needed.

## Upload to GitHub
1. Unzip this package.
2. Create a public GitHub repository, such as portfolio.
3. Choose Add file > Upload files. Upload index.html, background.html, the assets folder, the demos folder, and this README.md. Upload the contents, not the ZIP or an enclosing folder.
4. Commit to main.
5. Settings > Pages > Build and deployment: Deploy from a branch; main; /(root). Save.
6. Wait for the Pages deployment to complete. Test the resulting github.io URL, including demos and embeds.

The package also includes .nojekyll. If your file picker hides it, use Add file > Create new file and name it .nojekyll (an empty file is sufficient).

## Connect your current domain after testing
1. In repository Settings > Pages > Custom domain, enter lxd.amirfardbahreini.com and save. GitHub creates the CNAME file for branch publishing.
2. At your DNS provider, replace the current record for lxd with a CNAME pointing to YOUR-GITHUB-USERNAME.github.io. Do not include https:// or the repository name.
3. Once GitHub's DNS check succeeds and the certificate is ready, turn on Enforce HTTPS.
4. Check your domain before disconnecting it from Carrd. DNS can take up to 24 hours to update.

## Editing
index.html: main page, project descriptions, writing samples, feedback, and interactions.
background.html: interactive skills tree.
assets/: portrait and project visuals.
demos/: playable HTML experiences.

External Canva, YouTube, and calculator embeds need an internet connection.

## Git command alternative
Run these inside the extracted folder, replacing YOUR-GITHUB-USERNAME and portfolio with your actual values:

```sh
git init
git add .
git commit -m "Publish portfolio"
git branch -M main
git remote add origin https://github.com/YOUR-GITHUB-USERNAME/portfolio.git
git push -u origin main
```

Then enable Pages as described above.
