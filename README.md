# A4MP File Editor

A browser-based starter app for editing text content in PowerPoint `.pptx` files and editing `.txt`, `.csv`, and `.md` files.

## Features
- Upload a `.pptx` and inspect text areas extracted from slide XML.
- Edit extracted text and export an updated `.pptx` copy.
- Edit and download TXT, CSV, and Markdown text files.
- Responsive dark UI.
- GitHub Pages deployment workflow included.

## Requirements
- Node.js 20 or newer
- npm
- Git and a GitHub account (for publishing)

## Run locally
```bash
npm install
npm run dev
```
Open the local URL printed by Vite.

## Build
```bash
npm run build
```

## Publish on GitHub Pages

1. Create a **new public repository** on GitHub, for example `a4mp-file-editor`.
2. Extract this ZIP on your computer.
3. Open a terminal inside the extracted project folder and run:

   ```bash
   git init
   git add .
   git commit -m "Initial A4MP File Editor app"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/a4mp-file-editor.git
   git push -u origin main
   ```

   Replace `YOUR-USERNAME` with your GitHub username. If GitHub says the remote already exists, run `git remote set-url origin https://github.com/YOUR-USERNAME/a4mp-file-editor.git`.

4. On GitHub, open the repository → **Settings → Pages**.
5. Under **Build and deployment**, choose **GitHub Actions** as the source.
6. Open the **Actions** tab and wait for “Deploy A4MP File Editor to GitHub Pages” to complete successfully.
7. The live site URL will usually be `https://YOUR-USERNAME.github.io/a4mp-file-editor/`.

The included workflow runs automatically on each push to `main`. The exact URL depends on your GitHub username and repository name.

## Important limitations
This is a starter editor, not a full Microsoft PowerPoint replacement. It edits text found in many basic PPTX slide XML shapes, but may alter text-run formatting and does not render full slide layouts, edit images/charts/animations, or guarantee compatibility with every PPTX. DOCX/PDF/XLSX editing is not implemented. Files are processed in the browser; no backend or account system is included.
