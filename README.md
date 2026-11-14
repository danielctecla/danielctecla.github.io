# Daniel Catonga · Portfolio

Personal site and blog, built with [Astro](https://astro.build) and [Tailwind CSS](https://tailwindcss.com).

🌐 **Live:** [danielctecla.github.io](https://danielctecla.github.io)

## 🚀 Project Structure

```text
/
├── .github/workflows/
│   └── deploy.yml          # Builds and deploys to GitHub Pages on every push to main
├── public/
│   ├── assets/             # Images and documents served as-is
│   └── favicon.svg
├── src/
│   ├── components/         # Header, Footer, Intro, SectionContainer
│   ├── content/
│   │   └── blog/           # Blog posts in Markdown
│   ├── layouts/
│   │   └── Layout.astro
│   ├── pages/
│   │   ├── index.astro
│   │   └── blog/           # /blog and /blog/<post>
│   ├── styles/
│   │   └── global.css      # Tailwind theme (colors, fonts)
│   └── content.config.ts   # Blog collection schema
└── package.json
```

To learn more about the folder structure of an Astro project, refer to [the guide on project structure](https://docs.astro.build/en/basics/project-structure/).

## ✍️ Writing a blog post

Create a `.md` file in `src/content/blog/`. The file name becomes the URL (`my-post.md` → `/blog/my-post`).

```md
---
title: 'My post'
description: 'One line summary shown in the list.'
date: 2026-11-14
draft: false
---

Post content here.
```

Posts with `draft: true` are not published.

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## 📦 Deployment

Every push to `main` runs `.github/workflows/deploy.yml`, which builds the site with [`withastro/action`](https://github.com/withastro/action) and publishes it to GitHub Pages.

## 👀 Want to learn more?

Check the [Astro documentation](https://docs.astro.build) or the [Tailwind CSS documentation](https://tailwindcss.com/docs).
