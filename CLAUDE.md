# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is an academic portfolio website built using Jekyll and the Academic Pages theme. It's designed for showcasing academic work including publications, talks, teaching, and research projects. The site is deployed via GitHub Pages at https://amberxchen.github.io.

## Tech Stack

- **Static Site Generator**: Jekyll 3.x
- **Theme**: Academic Pages (based on Minimal Mistakes Jekyll theme)
- **Frontend**: HTML5, SCSS/CSS3, JavaScript (jQuery, FitVids, Magnific Popup)
- **Backend**: Ruby gems and Jekyll plugins
- **Deployment**: GitHub Pages
- **Containerization**: Docker with Ruby 3.2 base image

## Development Commands

### Local Development

**Install dependencies:**
```bash
bundle install
```

**Serve locally:**
```bash
bundle exec jekyll serve -l -H localhost
```
*Site will be available at http://localhost:4000*

**Alternative serve command (with config):**
```bash
jekyll serve -l -H localhost
```

### Docker Development

**Build and run with Docker Compose:**
```bash
docker compose up
```
*Site will be available at http://localhost:8000 (mapped from container port 4000)*

### Asset Building

**Build JavaScript assets:**
```bash
npm run build:js
```

**Watch JavaScript changes:**
```bash
npm run watch:js
```

**Manual uglify/minify:**
```bash
npm run uglify
```

### CV Management

**Update CV JSON from markdown:**
```bash
./scripts/update_cv_json.sh
```

## Site Architecture

### Directory Structure

- `_config.yml` - Main Jekyll configuration
- `_pages/` - Static pages (about, CV, publications, etc.)
- `_posts/` - Blog posts
- `_publications/` - Academic publication entries
- `_talks/` - Speaking engagement entries  
- `_teaching/` - Teaching experience entries
- `_news/` - News/announcement entries
- `_data/` - YAML data files (authors, navigation, CV JSON)
- `_layouts/` - Jekyll page layouts
- `_includes/` - Reusable Jekyll partials
- `_sass/` - SCSS stylesheets
- `assets/` - Static assets (CSS, JS, fonts, webfonts)
- `images/` - Image files
- `files/` - PDFs and other downloadable files
- `markdown_generator/` - Jupyter notebooks for generating markdown from TSV

### Content Collections

The site uses Jekyll collections for structured content:
- **Publications**: Academic papers with metadata (venue, date, citation, etc.)
- **Talks**: Conference presentations and invited talks
- **Teaching**: Course teaching experiences
- **Portfolio**: Project showcases
- **News**: Announcements and updates

### Key Configuration

- **Site URL**: https://amberxchen.github.io
- **Author Profile**: Configured in `_config.yml` under `author:` section
- **Social Links**: GitHub, Google Scholar, ORCID, Twitter
- **Collections**: Publications, talks, teaching, portfolio, news
- **Plugins**: Feed, sitemap, redirects, emoji support

### Layout System

- `default.html` - Base layout with header/footer
- `single.html` - Single page/post layout
- `archive.html` - Collection listing pages
- `talk.html` - Specialized layout for talk pages
- `cv-layout.html` - Custom CV page layout

### Asset Pipeline

- SCSS compilation via Jekyll
- JavaScript concatenation and minification via npm scripts
- jQuery, FitVids, Magnific Popup, and custom navigation scripts
- Academic icon fonts and Font Awesome integration

## Content Management

### Adding Publications

Create markdown files in `_publications/` with YAML frontmatter:
```yaml
---
title: "Paper Title"
collection: publications
category: manuscripts
permalink: /publication/paper-slug
date: 2024-01-01
venue: 'Journal Name'
citation: 'Author et al. (2024). Paper Title. Journal Name.'
---
```

### Adding Talks

Create markdown files in `_talks/` following similar pattern with talk-specific metadata.

### Content Generation

Use Jupyter notebooks in `markdown_generator/` to batch-generate markdown files from TSV data for publications and talks.

## Development Notes

- Jekyll configuration excludes development files (node_modules, vendor, etc.)
- Site builds automatically on GitHub Pages when pushed to master branch
- Local development requires Ruby, Bundler, and Node.js
- Docker provides isolated development environment
- CV can be maintained in markdown and converted to JSON for structured display
- Theme supports dark mode via `site_theme: "dark"` in config