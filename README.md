# Toan Quoc Nguyen: Academic Website

Single-file static site for GitHub Pages. No build step.

## Deploy

1. On GitHub, click **+ → New repository**. Owner: `toanquocnguyen`. Name: `toanquocnguyen.github.io`. Visibility: **Public** (required on GitHub Free).
2. Click **Add file → Upload files** and upload `index.html` (plus `photo.jpg` / `cv.pdf` if you add them) to the root of `main`. Commit.
3. Go to **Settings → Pages**. Under *Build and deployment*, choose **Deploy from a branch**, branch `main`, folder `/ (root)`, and save.
4. The site goes live at **https://toanquocnguyen.github.io**. Changes can take up to 10 minutes to appear.

Command line alternative:

```bash
git init && git add . && git commit -m "Initial site"
git branch -M main
git remote add origin https://github.com/toanquocnguyen/toanquocnguyen.github.io.git
git push -u origin main
```

## Edit

- **News:** add `<li>` items inside `<ul id="news-list">` (newest first) and delete the `<p class="empty">` line. A template is in the comment above the list.
- **Publications:** the `pubs` array near the bottom of `index.html`. Each entry takes `year`, `type`
  (`conf | journal | workshop | preprint`), `title`, `authors`, `venue`, and optional `pages`, `badge`,
  `doi`, `url`, `pdf`, `code`. Your name is bolded automatically. The list mirrors the publications in your CV.
- **Photo:** add `photo.jpg` and swap the `TN` placeholder in the `.avatar` div for
  `<img src="photo.jpg" alt="Toan Quoc Nguyen">`.
- **LinkedIn / CV:** uncomment and fill the placeholders in the hero links.
- Accent colors are defined once at the top of the `<style>` block: `--orange` (#EE442F) and `--blue` (#63ACBE).
