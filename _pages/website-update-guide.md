---
layout: single
title: "Website Update Guide"
permalink: /website-update-guide/
author_profile: true
---

# Website Update Guide

This guide documents how this portfolio website is structured and how to update it using the GitHub repository.

## 1. Repository Structure

The website is built with Jekyll and the Academic Pages template.

Key directories include:

- `_pages/` — standalone website pages such as About, Experience, Research, and CV.
- `_portfolio/` — AI projects and portfolio items.
- `_publications/` — publications and academic outputs.
- `_data/` — site data such as the navigation menu.
- `files/` — downloadable files such as a CV PDF.

## 2. Updating the Navigation

The main navigation is controlled by:

`_data/navigation.yml`

Each navigation item contains a display title and a URL. For example:

```yaml
- title: "Experience"
  url: /experience/
```

## 3. Adding an Experience

Create a Markdown file under `_pages/` with front matter containing a title and permalink.

Example:

```yaml
---
layout: single
title: "Experience"
permalink: /experience/
author_profile: true
---
```

## 4. Adding an AI Project

AI projects are stored in the `_portfolio/` collection. Each project can be created as a Markdown file with `collection: portfolio` in its front matter.

## 5. Adding a Publication

Publications are stored in `_publications/`. Academic Pages uses the collection metadata to generate publication pages and publication lists.

## 6. Updating the CV

The main CV page is `_pages/cv.md` and is available at `/cv/`. Academic Pages can also generate sections dynamically from collections such as publications, talks, and teaching.

## 7. GitHub Pages Deployment

After changes are committed to the repository, GitHub Pages builds the Jekyll site and publishes the generated website.

## 8. Recommended Update Workflow

1. Make a small, focused change.
2. Commit the change with a clear message.
3. Wait for the GitHub Pages build to complete.
4. Open the live website and verify the affected page.
5. Check navigation links and formatting before making the next change.
