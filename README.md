# tonybowen.me

Personal blog built with [Astro](https://astro.build). Static HTML, Markdown posts, zero client-side JavaScript (except a tiny theme toggle).

## Local development

```bash
npm install
npm run dev
```

Opens at `http://localhost:4321`.

## Adding a new blog post

1. Create a new `.md` file in `src/content/blog/`, e.g. `src/content/blog/my-new-post.md`.
2. Add frontmatter at the top:

```markdown
---
title: "My New Post"
date: 2026-03-15
description: "A short summary that appears on the home page."
---

Your content here...
```

3. That's it. The post will automatically appear on the home page sorted by date (newest first).

### Adding images

Place images in `public/images/` and reference them in Markdown:

```markdown
![Alt text](/images/my-photo.jpg)
```

### Embedding YouTube videos

Use an iframe wrapped in the `video-embed` class for responsive 16:9 sizing:

```html
<div class="video-embed">
  <iframe
    src="https://www.youtube.com/embed/VIDEO_ID"
    title="Video title"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
  </iframe>
</div>
```

## Build

```bash
npm run build
```

Output goes to `dist/`.

## Deploy on Render

1. Push this repo to GitHub.
2. Go to [Render](https://render.com) and create a new **Static Site**.
3. Connect your GitHub repo.
4. Set these values:
   - **Build command:** `npm run build`
   - **Publish directory:** `dist`
5. Deploy.

Render will rebuild automatically on every push to the connected branch.

## Project structure

```
src/
  content/
    blog/          <- Markdown posts go here
  layouts/
    Base.astro     <- Shared HTML shell (head, header, footer)
  pages/
    index.astro    <- Home page
    blog/
      [...slug].astro  <- Individual post pages
  styles/
    global.css     <- All styling
  content.config.ts  <- Content collection schema
public/
  images/          <- Static images
  favicon.svg
```
