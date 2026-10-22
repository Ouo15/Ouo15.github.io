# Frederic OKE-AGBO — personal website

Built with [Quarto](https://quarto.org), deployed to <https://ouo15.github.io> by GitHub Actions.

## Write a new post

1. Create a folder: `posts/my-post-name/`
2. Add `posts/my-post-name/index.qmd`:

   ```yaml
   ---
   title: "My post title"
   description: "One-sentence summary shown on the blog page."
   date: "2026-10-20"
   categories: [Machine Learning, Python]
   image: thumbnail.png   # optional card image, placed in the same folder
   ---
   ```
3. Preview while writing: `quarto preview`
4. Render: `quarto render` (runs your code and updates `_freeze/`)
5. Publish: `git add . && git commit -m "New post" && git push`

Always render before pushing: GitHub does not run your Python/R code, it
reuses the results saved in `_freeze/`.

## Where things live

| File | What it is |
|------|------------|
| `_quarto.yml` | Site settings, navbar, social links |
| `index.qmd` | Home page |
| `about.qmd`, `cv.qmd` | About and CV pages |
| `projects.yml` | Project cards on the Projects page |
| `posts/` | Blog posts (one folder each) |
| `styles/` | Colors and fonts (light + dark) |
| `images/` | Profile photo, favicon |
