# chroma-db-web

Public assets and GitHub Pages site for [Chroma DB](https://marketplace.visualstudio.com/items?itemName=harishkaparwan.chroma-db).

Live at: **https://harishkaparwan.github.io/chroma-db-web/**

## Structure

```
index.html          ← Landing page (served at root)
app/                ← Built React workbench (populated by deploy:web)
public/
  assets/           ← Logo, walkthrough GIF, and static images
  Desktop/          ← Tauri/macOS desktop icon assets
  policy/
    privacy.html    ← Privacy Policy
  webpage/          ← Static plugin home page assets
.github/workflows/
  deploy.yml        ← GitHub Pages deploy workflow (GitHub Actions)
```

## Deploying the web workbench

From the private `chroma-db` source repo:

```bash
npm run deploy:web
```

This builds the React app with base `/chroma-db-web/app/` and copies the output into `chroma-db-web/app/`. Then commit and push `chroma-db-web`.
