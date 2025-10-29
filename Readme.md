## AERA93-GradNetwork

Static site built with Quarto for the AERA93 Graduate Network. This repository contains source `.qmd` files and the generated site under `docs`.

### About the Website

The site is the public home for the AERA93 Graduate Network. It shares timely announcements, timelines, events, and key links for members and supporters. Visitors can learn who we are, send suggestions to help improve the network, and opt out of future outreach emails if they prefer.

What you'll find on the site:

- Home: highlights, news, timelines, and important links
- Who We Are (`whoweare.qmd`): brief overview of the Graduate Network
- Suggestions (`suggestions.qmd`): simple form to share feedback or ideas
- Unsubscribe (`unsubscribe.qmd`): quick opt-out for email communications

### Purpose

- Provide a simple, fast public homepage for the AERA93 Graduate Network
- Share announcements, timelines, and key links in one place
- Collect feedback via the suggestions form (`suggestions.qmd`)
- Offer an opt-out link for emails via the unsubscribe page (`unsubscribe.qmd`)
- Serve as a lightweight, version-controlled record of site content

### Project Structure

- `_quarto.yml`: Quarto project/site configuration
- `index.qmd`, `whoweare.qmd`, `suggestions.qmd`, `unsubscribe.qmd`: Source pages
- `styles.css`: Custom styles used by the site
- `docs/`: Rendered output (HTML, assets)

### Prerequisites

- Quarto: install from `https://quarto.org`
- Optional: Pandoc is bundled with Quarto; no separate install needed

### Common Commands

- Preview the site with live reload:
  ```bash
  quarto preview
  ```

- Render the site to `docs/`:
  ```bash
  quarto render
  ```

### Editing Content

- Edit `.qmd` files (e.g., `index.qmd`) using Markdown and Quarto shortcodes.
- Global settings like theme and navigation live in `_quarto.yml`.
- Customize styles in `styles.css` (a copy is also in `docs/styles.css` but edit the root file).

### Deployment

The `docs/` directory contains the static output and is deployed at GitHub Pages. For GitHub Pages from `main`:

1. Render locally: `quarto render`
2. Serve `docs/` via Pages (e.g., set Pages to use the `/docs` folder from the `main` branch) or publish with Quarto:
   ```bash
   quarto publish gh-pages
   ```

### Contributing

1. Create a branch
2. Make edits to `.qmd`/`_quarto.yml`/`styles.css`
3. Run `quarto preview` to verify
4. Open a pull request