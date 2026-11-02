# Rokonozzaman Ayon — Research Portfolio

Academic portfolio of **Rokonozzaman Ayon**, an AI/ML researcher based in Dhaka, Bangladesh. The site presents publications, research datasets, projects, education, experience, academic service, and contact details in a single newspaper-style page.

## Highlights

- **Publications:** filter by category (All, Journal, Conference, Preprint, Ongoing), search by title, venue or tag, and see each paper's status.
- **Research datasets:** published Mendeley Data records with direct links, plus datasets in preparation.
- **Projects:** research prototypes and production systems.
- **Academic service:** peer-review record by journal, linked to ORCID.
- **Light and dark themes:** follows the visitor's system setting, with a manual toggle.
- **Motion:** subtle reveal and hover effects, all turned off when a visitor's device asks for reduced motion.
- **Responsive:** works on desktop, tablet and phone.

## Tech

- One self-contained `index.html` with no build step and no framework.
- Plain HTML, CSS and JavaScript.
- [three.js](https://threejs.org/) (r128, loaded from cdnjs) draws the animated network in the header.
- Google Fonts: Cormorant Garamond, Lora and DM Sans.

## Repository structure

```
index.html   The complete site: styles, content data and scripts
README.md    This file
```

## Updating the content

All content lives as JSON in a single block near the end of `index.html`:

```html
<script type="application/json" id="portfolio-data"> … </script>
```

Edit that JSON (profile, figures, links, and the `sections` list), save, and the page renders the new content on its next load. Each section has a `type` that sets its layout: `publications`, `projects`, `datasets`, `timeline`, `experience`, `skills`, `service`, `entries`, `text` or `contact`.

> The built-in visual editor (the "Edit portfolio" button) only works when the page is opened as a Claude artifact. On GitHub Pages the site is read-only, so edit the JSON directly.

## Deployment

The site is ready for GitHub Pages:

1. Open **Settings → Pages** in this repository.
2. Under **Build and deployment**, choose **Deploy from a branch**, then select `main` and `/ (root)`.
3. Save. The site is published at `https://rokayon.github.io/ayon/`.

To preview locally, open `index.html` in any modern browser.

## Contact

- Email: rokayon.cse@gmail.com
- Google Scholar: [profile](https://scholar.google.com/citations?user=7JU3jzsAAAAJ)
- ORCID: [0009-0000-3602-0714](https://orcid.org/0009-0000-3602-0714)
- LinkedIn: [rokonozzaman-ayon](https://www.linkedin.com/in/rokonozzaman-ayon/)

© 2026 Rokonozzaman Ayon. All rights reserved.
