# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with this repository.

## Project Overview

This is Saeed Semrin's personal website hosted on GitHub Pages at `saeedsemrin.github.io`. It's a static site with a minimalist design featuring a blog, bio, contact page, and workout log.

## Project Structure

```
/
├── index.html          # Homepage with links, time display, and location
├── bio.html            # About/biography page
├── blog.html           # Blog listing page
├── contact.html        # Contact information page
├── workout-log.html    # Workout tracking page
├── style.css           # Main stylesheet
├── style_blog.css      # Blog-specific styles
├── blog/               # Individual blog posts (HTML files)
│   └── template.html   # Template for new blog posts
├── docs/               # Documentation/assets
├── picasso.png         # Logo image
├── favicon.ico         # Site favicon
└── CNAME               # Custom domain configuration
```

## Design System

- **Font**: Courier Bold / Courier New (monospace)
- **Primary Color**: Blue (#0000ff) for all links
- **Background**: White (#ffffff)
- **Accent**: Golden yellow (#ffd700) for name highlight
- **Link Style**: Underlined, separated by `|` pipes in navigation

## Development Guidelines

### Adding Blog Posts
1. Copy `blog/template.html` as a starting point
2. Name the file descriptively with hyphens (e.g., `my-new-post.html`)
3. Add an entry to `blog.html` to list the new post
4. Blog posts use `style_blog.css` for styling

### Styling Conventions
- All pages should use Courier/monospace font family
- Links are always blue (#0000ff) and underlined
- Keep the minimalist aesthetic - avoid adding complex UI elements
- Pages use flexbox for centering content

### Static Site
- No build process required - all files are plain HTML/CSS
- JavaScript is used sparingly (time display, location fetch on homepage)
- Changes deploy automatically when pushed to the main branch

## Common Tasks

- **Preview locally**: Open any HTML file directly in a browser
- **Deploy**: Push changes to the main branch - GitHub Pages auto-deploys
- **Add new page**: Create HTML file, link from index.html or relevant page
