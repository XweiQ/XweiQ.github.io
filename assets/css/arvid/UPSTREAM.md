# Arvid Academic Homepage Template

Source: https://github.com/Arvid-pku/Academic-Homepage-Template
Revision: a2fcbe3450cdf637a91a156468dc312dbe9ddfe0

- stylesheet.css and shared-styles.css: upstream copies with the content width increased to 960px.
- homepage.css: upstream index.html style block, with the requested compact
  publication spacing appended to match the Publications page.
- ../../js/arvid/utils.js: unchanged upstream copy.
- ../../js/arvid/site-shell.js: upstream file with navigation targets, author,
  social profile URLs and footer attribution adapted to Xiaowei Qian.
- Homepage markup follows the upstream profile and publication structure.
- Content is rendered with Jekyll from the existing biography and publications.
- All original navigation tabs are retained with Jekyll pages. Blogs and
  Photography show empty states until personal content is added.
- Page-specific CSS is extracted unchanged from the corresponding upstream
  HTML files; blog-styles.css is an unchanged upstream copy.
- Existing education and research experience use the dated-list component.
- Publication order: title, authors, then venue/year and links. Long text wraps.

The upstream repository did not contain a LICENSE file at this revision.
Source and authorship are retained here. The visible footer credit was removed
at the site owner's request.

Local updates: Projects and CV currently retain only their page headings.
Publications uses Preprints and Conference groups, with compact uniform line
spacing in publications.css at the owner's request. Other page CSS remains unchanged.

Typography consolidation: typography.css owns the shared type scale, colors,
line height and spacing. homepage.css now contains layout only; the Publications
page uses the same typography rules. Original upstream sources remain identified above.
