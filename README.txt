AN_Gen v15 Hidden Template Fix

Why the extra blank page appeared:
- The blank page is the hidden HTML page template used by JavaScript to clone new pages.
- Because the CSS gives .page display:flex, iPhone/Safari can override the hidden attribute and print the template.
- The blank page usually shows the default title, often "Residential Internet 2026", with no body content.

Fix:
- Adds a hard CSS rule:
  [hidden], #pageTemplate { display:none !important; }
- Applies the same rule inside @media print.

Upload these files to GitHub:
- index.html
- app-v15.js
- an-gen-v15.css
- IncludedSectionContent.csv
- Sparklight_R-purple-rgb.png
- Sparklight_R-Business-purple-rgb.png
