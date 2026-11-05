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
- **Scholar mascot:** a small character in the bottom-right corner greets visitors, points them to the research and contact sections, reacts to searches and copied emails, and tucks out of the way while they scroll. It can be turned off or reworded in the editor.

## Tech

- One self-contained `index.html` with no build step and no framework.
- Plain HTML, CSS and JavaScript.
- [three.js](https://threejs.org/) (r128, loaded from cdnjs) draws the animated network in the header.
- Google Fonts: Cormorant Garamond, Lora and DM Sans.
- [Bible Strong Avatar Lab](https://github.com/smontlouis/bible-strong-avatar-lab) (`@bible-strong/avatar-web` 0.1.0) renders the mascot. It is bundled into the page.

## Repository structure

```
index.html               The complete site: styles, content data, mascot engine and scripts
LICENSE                  GNU Affero General Public License v3.0 (applies to the code)
THIRD_PARTY_NOTICES.md   Credits and licences for bundled and loaded third-party software
licenses/                Licence texts for bundled third-party packages
README.md                This file
```

## Updating the content

### With the built-in editor

1. Open the site and click **Edit** in the footer.
2. Enter the editor password.
3. Make your changes. Every section, entry, link, figure and the portrait can be added, edited, reordered, hidden or deleted.
4. Click **Download page**. Your browser saves an updated `index.html`.
5. Upload that file to this repository, replacing the old `index.html`. The live site updates after GitHub Pages rebuilds.

Edits stay in your browser until you download the page, so nothing changes for visitors until you upload the new file. When the page is opened as a Claude artifact instead, the same editor publishes changes directly.

### By hand

All content lives as JSON in a single block near the end of `index.html`:

```html
<script type="application/json" id="portfolio-data"> … </script>
```

Each section has a `type` that sets its layout: `publications`, `projects`, `datasets`, `timeline`, `experience`, `skills`, `service`, `entries`, `text` or `contact`.

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

## Credits

The mascot is rendered with [Bible Strong Avatar Lab](https://github.com/smontlouis/bible-strong-avatar-lab) by Stéphane Montlouis-Calixte, licensed under the GNU AGPL v3.0. Its character definition is adapted from that project's Strobi example. Full details and all other third-party licences are in [THIRD_PARTY_NOTICES.md](./THIRD_PARTY_NOTICES.md).

## Licence

- **Code:** the site's code includes AGPL-3.0 software, so the code in this repository is released under the [GNU Affero General Public License v3.0](./LICENSE). Its source is this repository, which the site's footer links to.
- **Content:** the biography, publication and dataset records, project descriptions and portrait photograph are © 2026 Rokonozzaman Ayon and are not covered by the code licence. Please ask before reusing them.
