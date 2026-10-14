# DART Project Website

This repository hosts the static website for **DART – Intelligent Detection, Response and Analysis of Security Events**, a VLAIO TETRA project carried out by KU Leuven DistriNet (Campus Gent, project lead) and the VUB Software Languages Lab (SOFT).

🌐 **Live Site:** [https://dart.projects.cybersecurity-research.be](https://dart.projects.cybersecurity-research.be)

## About the Project

DART helps Flemish SMEs, non-profits and their service providers build feasible, NIS2-aligned detection and incident response capabilities. The project delivers:
- A practical framework for interpreting cyber risks and legal obligations (NIS2, GDPR)
- Guidelines, workflows and playbook templates for detection, triage, response and reporting
- Reference architectures and an open repository of detection rules and automation playbooks
- A testbed with demonstrators, and the practical guide *"From Detection to Response"*

## Website Structure

Built with Jekyll and GitHub Pages.

- **Home** (`index.md`): project overview
- **Project** (`project.md`): work packages and deliverables
- **Knowledge Dissemination** (`knowledge-dissemination.md`): meetings, events, publications and results
- **Partners** (`consortium.md`): research partners, contacts and advisory group
- **Blog** (`blog.md`, posts in `_blog/`): articles, not in the main navigation

Placeholders that still need content are marked with `TODO` comments or `[Name]` / `Date TBA`:

```bash
grep -rn "TODO\|\[Name\]\|TBA" --include=*.md --include=*.html --include=*.yml .
```

## Running Locally

```bash
gem install bundler
bundle install
bundle exec jekyll serve
# Visit http://localhost:4000
```

## Adding Content

### An advisory group meeting

Edit the matching section in `knowledge-dissemination.md`: replace `Date TBA` and fill in the agenda.

### An event with presentations

1. Put the PDFs in `assets/events/<YYYY_MM_DD name>/` (PDFs are stored with Git LFS).
2. Create `_dissemination/<YYYY-MM-DD-name>.md`:

   ```markdown
   ---
   layout: event
   title: "Event title"
   date: 2027-01-15
   event_type: "Advisory Group Meeting + Workshop"
   ---

   # Event title

   **Date:** January 15, 2027
   **Location:** ...

   ## Presentations

   {% include presentation-card.html
      href="/assets/events/2027_01_15%20Kickoff/1.%20Intro.pdf"
      title="Introduction"
      speaker="J. Doe"
      company="Optional company" %}
   ```

The event is listed automatically under *Event Materials* on the Knowledge Dissemination page.

### A blog post

Create `_blog/<name>.md`:

```markdown
---
layout: blog
title: "Post title"
author: J. Doe
date: 2027-01-15
reading_time: "5 min read"
excerpt: "One-sentence summary."
author_ico: "/assets/images/<avatar>.jpg"
---

Content...
```

To show the blog in the navigation, add `blog.md` to `header_pages` in `_config.yml`.

### Partners and logos

Edit `consortium.md` for partner descriptions, contacts and the advisory group. Logos go in `assets/images/`; the footer is in `_includes/footer.html`. The header uses a text logo (`_includes/header.html`); swap in an image once a DART logo exists.

## Deployment

Pushing to `main` triggers the GitHub Actions workflow, which builds the site and deploys it to GitHub Pages. The custom domain is set in `CNAME`.

## License

Content © KU Leuven - DistriNet and VUB - Software Languages Lab. All rights reserved.
