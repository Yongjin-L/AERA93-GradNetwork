## AERA93-GradNetwork

Static site built with Quarto for the AERA93 Graduate Network. This repository contains source `.qmd` files and the generated site under `_site/`.

### Project Structure

- `_quarto.yml`: Quarto project/site configuration
- `index.qmd`, `suggestions.qmd`, `unsubscribe.qmd`: Source pages
- `styles.css`: Custom styles used by the site
- `_site/`: Rendered output (HTML, assets)

### Prerequisites

- Quarto: install from `https://quarto.org`
- Optional: Pandoc is bundled with Quarto; no separate install needed

### Common Commands

- Preview the site with live reload:
  ```bash
  quarto preview
  ```

- Render the site to `_site/`:
  ```bash
  quarto render
  ```

### Editing Content

- Edit `.qmd` files (e.g., `index.qmd`) using Markdown and Quarto shortcodes.
- Global settings like theme and navigation live in `_quarto.yml`.
- Customize styles in `styles.css` (a copy is also in `_site/styles.css` but edit the root file).

### Deployment

The `_site/` directory contains the static output and can be deployed to any static host (e.g., GitHub Pages, Netlify). For GitHub Pages from `main`:

1. Render locally: `quarto render`
2. Serve `_site/` via Pages (e.g., set Pages to use the `/_site` folder from the `main` branch) or publish with Quarto:
   ```bash
   quarto publish gh-pages
   ```

### Contributing

1. Create a branch
2. Make edits to `.qmd`/`_quarto.yml`/`styles.css`
3. Run `quarto preview` to verify
4. Open a pull request

### License

Unless otherwise noted, content is provided under an open content license typical for documentation sites. Update this section with the specific license if required.
