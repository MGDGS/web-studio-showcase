# Web Studio Showcase

A bilingual (English / 简体中文) portfolio for an independent website developer, with restaurant, nail salon and barbershop concept demos. Built with HTML, CSS and vanilla JavaScript, without a build dependency.

## Pages

- `index.html`: studio introduction, industry filters, demo collection, process and contact placeholders.
- `restaurant.html`: menu category filtering and table reservation preview.
- `nails.html`: services, image gallery and appointment preview.
- `barber.html`: services, image gallery and appointment preview.

Language selection is saved in browser local storage. Booking forms validate required fields and dates, reject closed Mondays, and display a local preview. No data is transmitted, stored on a server or emailed. These are fictional concept businesses; imagery, prices, locations and hours are illustrative.

## Customize

Edit copy, service data and placeholder contact/pricing content in `assets/app.js`. Change visual styles in `assets/style.css`, and replace images in `assets/`. `build.py` regenerates the four HTML entrypoints; no build step is required to publish.

## Preview

Run `python3 -m http.server 8000` in this directory, then open http://localhost:8000.

## Deployment

GitHub Actions deploys on pushes to `main` with `.github/workflows/pages.yml`. In repository Settings → Pages, set the source to **GitHub Actions**. All asset and page links use relative paths to support a GitHub Pages project site.

## Images and typography

Illustrative photography from Unsplash; original URLs are recorded in `assets/image-sources.json`. Photos are downloaded locally so they do not depend on a remote photo host at runtime. Images are not claimed as work by the fictional businesses. Google Fonts supplies DM Sans and Playfair Display; system fonts are available as fallbacks.

## Personal website demos

- `blog.html`: bilingual journal with category filters and sample article dialogs.
- `birthday.html`: birthday greeting with a surprise message and memory gallery.
- `portfolio.html`: fictional designer portfolio with concept-project details.

The homepage supports Business and Personal filters across all six demos. Personal templates and interactions live in `assets/personal.js`. Portfolio artwork is an original inline SVG/CSS composition; sample names and project stories are fictional.
