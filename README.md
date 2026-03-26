# Personal Website

Minimalistic personal site. Pure HTML/CSS — no build step, no dependencies.

## Structure

```
index.html              ← homepage
links.html              ← links page
blog/
  index.html            ← blog listing
  posts/
    hello-world.html    ← posts live here
style.css               ← shared styles (one file for everything)
```

## Adding a new blog post

1. Copy `blog/posts/hello-world.html` to a new file: `blog/posts/your-post-slug.html`
2. Update the `<title>`, `<h1>`, date, reading time, and body content
3. Add a new entry to `blog/index.html`:
   ```html
   <li>
     <span class="date">YYYY-MM-DD</span>
     <a href="posts/your-post-slug.html">Your post title</a>
   </li>
   ```
   Posts are listed newest first — add the new entry at the top of the `<ul>`.

## Deployment

Served via GitHub Pages from this folder, or move to a dedicated repo for a custom domain.
