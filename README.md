# jozefsedlak.com

My personal website: blog, portfolio and hobby projects.

Built with [Astro](https://astro.build), hosted on Cloudflare (Workers static assets). Every push to `main` publishes the site automatically.

## Where things live

| Folder | What goes there |
| --- | --- |
| `src/content/blog/` | Blog posts, one Markdown (`.md`) file each |
| `src/content/projects/` | Portfolio and hobby projects, one Markdown file each |
| `src/pages/` | Site pages (home, about, blog and project lists) |
| `src/layouts/` | Shared page frame (header, nav, footer) |
| `src/styles/global.css` | Colours and typography |
| `public/` | Images and files served as-is (e.g. `public/images/photo.jpg` → `/images/photo.jpg`) |

## Writing a new post

Create `src/content/blog/my-post.md`:

```md
---
title: My post
description: One-line summary.
date: 2026-11-24
draft: false
---

Text goes here.
```

Set `draft: true` to keep it off the site until it's ready.

## Running locally (optional)

Needs [Node.js](https://nodejs.org) 22+.

```sh
npm install     # once, downloads dependencies
npm run dev     # live preview at http://localhost:4321
npm run build   # production build into dist/
```
