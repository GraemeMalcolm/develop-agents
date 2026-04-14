---
title: Module  title
description: Module description.
level: 200
published: false
---

# Template for GitHub-based Content

This is a template repository for creating GitHub-based skilling content that renders as a GitHub Pages site.

## Setup Instructions

1. **Update module metadata**: Edit `_data/module.yml` to set your module title, description, and level.

2. **Add content**: Create markdown files in the `content/` folder. Each file should have frontmatter with:
   - `layout: content`
   - `title:` (topic title)
   - `description:` (topic description)
   - `duration:` (estimated minutes)

3. **Add media**: Place images and other media in `content/media/`

4. **Enable GitHub Pages**: In your repository settings, enable GitHub Pages and set the source to the main branch.

The site will automatically generate a landing page with links to all content pages, and navigation between pages.
