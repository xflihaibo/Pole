---
title: Docsify Bookmark Blog Initialization
type: note
permalink: implementations/docsify-bookmark-blog-initialization
---

Implemented a docsify-based bookmark collection blog.
Project Structure:
- `docs/index.html`: Main entry point with custom CSS for bookmark cards and standard plugins (search, copy-code, pagination).
- `docs/README.md`: Homepage with a featured bookmark grid using custom HTML classes.
- `docs/_sidebar.md`: Sidebar configuration.
- `docs/.nojekyll`: Deployment configuration for GitHub Pages.

Patterns:
- Used custom CSS classes (`bookmark-grid`, `bookmark-card`) to create a card-like layout for links.
- Configured docsify with `loadSidebar: true` for better navigation.
