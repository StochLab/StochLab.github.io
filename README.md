# Stoch Lab Website

Source repository for the [Stochastic Robotics Lab website](https://www.stochlab.com/). The site is built with Jekyll and published from the `master` branch through GitHub Pages.

## Update Rules

- Make content changes in source files only. Do not edit generated files in `_site/` or `.jekyll-cache/`.
- Keep changes focused and use relative site paths such as `/img/people/name.jpg` for local assets.
- Add images and videos under `img/` and commit them with the page or data-file change that references them.
- Preserve existing YAML indentation. Use two spaces for list items and do not use tabs.
- Preview every visual or content change locally before publishing.
- Check `git status` before committing. Do not include `_site/`, `.jekyll-cache/`, or unrelated local changes.

## Local Setup And Preview

Requirements: Ruby and Bundler. Python is also needed only when rebuilding the legacy BibTeX include with `make`.

```sh
bundle install
bundle exec jekyll serve
```

Open <http://127.0.0.1:4000>. To use the Makefile's local server instead, run `make serve`; it serves at <http://127.0.0.1:5000> and may regenerate `_includes/pubs.html`.

Before publishing, verify the production build:

```sh
bundle exec jekyll build
```

## Common Content Updates

### People

Edit `_data/people.yml`. Each entry needs a unique key, `display_name`, and a valid `role`. Optional fields include `webpage`, `github`, `image`, and `bio`.

```yaml
newperson:
  display_name: "New Person"
  role: phd
  webpage: "https://example.com/"
  image: /img/people/new-person.jpg
  bio: Research area or program
```

Available roles are defined in `_config.yml`. To move someone to alumni or past interns, change only their `role` and update their `bio` as appropriate.

### News

Create a file in `_posts/` named `YYYY-MM-DD-short-title.md`. The filename date controls ordering, so use the announcement date. Use `shortnews: true` for announcements displayed directly in the news feed.

```markdown
---
title: Announcement title
layout: post
shortnews: true
icon: newspaper-o
---

Announcement text.
```

Use a descriptive `title` and omit `shortnews` for a full blog post. Do not use a future date unless the item should remain hidden until that date.

### Research Projects

Create or edit a Markdown file in `_projects/`. Project cards are ordered by `last-updated`, newest first. Set `status: inactive` to hide a project from the active project listings.

```yaml
---
title: Project title
description: Short card description.
people:
  - person-key
layout: project
image: /img/project-image.jpg
last-updated: 2026-08-12
category: learning
---
```

The `people` values must match keys in `_data/people.yml`, and `category` must match a research-area key in `_data/areas.yml`.

### Research Areas, Sponsors, And Publications

- Edit `_data/areas.yml` for research-area names, copy, and media.
- Edit `_data/sponsors.yml` and add the matching logo under `img/funding/` for funding updates.
- Edit `_data/pubs.yml` for the publications page. Preserve the existing record structure and confirm the entry appears in the correct year and section.

### Site-Wide Configuration

Edit `_config.yml` only for configuration shared across the site, including navigation, homepage news count, people roles, and Jekyll settings. Review all pages affected by a configuration change.

## Publish

After the local build succeeds and the preview looks correct, commit the intended source changes and push to `master`:

```sh
git status
git add <intended-files>
git commit -m "Update website content"
git push origin master
```

GitHub Pages deploys the `master` branch. Confirm the update at <https://www.stochlab.com/> after the GitHub Pages build completes.
