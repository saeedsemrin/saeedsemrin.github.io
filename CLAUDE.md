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
├── workout-log.html    # Workout tracking page (weekly grid view)
├── 404.html            # Custom 404 error page
├── style.css           # Main stylesheet
├── style_blog.css      # Blog-specific styles
├── blog/               # Individual blog posts (HTML files)
│   └── template.html   # Template for new blog posts
├── docs/               # Documentation/assets
├── picasso.png         # Logo image (actually WebP format)
├── favicon.ico         # Site favicon
└── CNAME               # Custom domain configuration (saeedsemrin.com)
```

## Design System

- **Font**: Arial, sans-serif
- **Primary Color**: Blue (#0000ff) for all links
- **Background**: White (#ffffff)
- **Accent**: Golden yellow (#ffd700) for name highlight
- **Link Style**: Underlined, separated by `|` pipes in navigation
- **Mobile**: Responsive design with breakpoints at 768px

## Development Guidelines

### Adding Blog Posts
1. Copy `blog/template.html` as a starting point
2. Name the file descriptively with hyphens (e.g., `my-new-post.html`)
3. Update the `<head>` section with proper title, meta description, and OG tags
4. Add an entry to `blog.html` to list the new post (include share links)
5. Blog posts use `style_blog.css` for styling

### Styling Conventions
- All pages should use Arial sans-serif font family
- Links are always blue (#0000ff) and underlined
- Keep the minimalist aesthetic - avoid adding complex UI elements
- Pages use flexbox for centering content
- Include favicon on all pages: `<link rel="shortcut icon" type="image/x-icon" href="/favicon.ico">`

### SEO Requirements
All pages should include:
- `<meta name="description">` tag
- Open Graph tags (og:title, og:description, og:image, og:url, og:type)
- Descriptive `<title>` with format: "page name | saeed semrin"

### Static Site
- No build process required - all files are plain HTML/CSS
- JavaScript is used sparingly (time display, location fetch on homepage)
- Changes deploy automatically when pushed to the main branch

## Common Tasks

- **Preview locally**: Open any HTML file directly in a browser
- **Deploy**: Push changes to the main branch - GitHub Pages auto-deploys
- **Add new page**: Create HTML file, link from index.html or relevant page
