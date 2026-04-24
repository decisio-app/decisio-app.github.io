# Decisio Landing Page

Landing page for [Decisio: AI Decision Maker](https://apps.apple.com/app/id6752439703) iOS app.

**Live site:** https://decisio-app.github.io

## Structure

This site uses **Jekyll** for templating. All analytics (Google Analytics, Amplitude) are centralized in `_includes/`.

```
_config.yml          # Jekyll configuration
_includes/
  analytics.html     # Google Analytics (GA4)
  amplitude.html     # Amplitude tracking
  favicon.html       # Favicon
  apple-banner.html  # Apple Smart App Banner
_layouts/
  landing.html       # Main landing page layout
  compare.html       # Comparison pages layout
  blog.html          # Blog posts layout
  decide.html        # Decision tool pages layout
  page.html          # Generic page layout
```

## Adding a New Page

1. Create an HTML file with Jekyll front matter:

```html
---
layout: compare
title: "Decisio vs NewApp - Comparison"
description: "Compare Decisio and NewApp..."
canonical: "https://decisio-app.github.io/compare/newapp"
---
<style>
/* Your page styles */
</style>
<body>
<!-- Your content -->
</body>
```

2. The layout automatically includes:
   - Google Analytics (G-4M8W8YY7M9)
   - Amplitude tracking
   - Open Graph / Twitter Card meta
   - Apple Smart App Banner
   - Favicon

## Local Development

```bash
bundle install
bundle exec jekyll serve
```

## Deployment

Push to `main` branch. GitHub Pages automatically builds and deploys.
