# Template sources and local adaptations

## Current visual template

- Project: [Arvid Academic Homepage Template](https://github.com/Arvid-pku/Academic-Homepage-Template)
- Imported revision: `a2fcbe3450cdf637a91a156468dc312dbe9ddfe0`
- Reference: https://arvid-pku.github.io/Academic-Homepage-Template/index.html

The upstream layout, navigation, base styles, page-specific styles, and utility scripts were adapted to this Jekyll website. These files are maintained local copies, not an automatically synchronized upstream checkout.

### Local changes

- Jekyll layouts: `_layouts/home.html` and `_layouts/arvid-page.html`.
- Shared paper data and rendering: `_data/publications.yml` and `_includes/arvid-paper.html`.
- `typography.css`: independent heading/body/interface fonts, burgundy and ink-blue roles, type scale, compact spacing, underlined author name, and paper distinctions.
- `homepage.css`: profile/photo grouping, full-width biography, and inline education entries.
- `shared-styles.css`: common page/navigation width and responsive gutters.
- `site-shell.js`: personal links, local navigation routes, and adapted footer; dark-mode button temporarily commented out.
- `utils.js`: upstream dark-mode, icon, and back-to-top utilities retained. Dark-mode initialization is commented out in both layouts.
- Original page tabs retained; Projects and CV intentionally empty, Blogs and Photography placeholders.
- CSS and JavaScript URLs in both layouts include a build version to refresh caches after deployment.

The referenced Arvid revision contained no LICENSE file. This note preserves its source and authorship; the historical repository MIT license is not a claim about the licensing of imported Arvid assets.

## Historical Jekyll foundation

The earlier version used [AcadHomepage](https://github.com/RayeRen/acad-homepage.github.io). Some Jekyll infrastructure and legacy files remain from that version. Their existing copyright and license notices, including the root LICENSE, are retained. AcadHomepage is not the current visual template.

## Typography references

[Tufte CSS](https://edwardtufte.github.io/tufte-css/) informed typography experiments. Current headings and body use Palatino; interface text uses Gill Sans with system fallbacks. ET Book font files are retained for optional future use with their own LICENSE in `assets/fonts/et-book/`.
