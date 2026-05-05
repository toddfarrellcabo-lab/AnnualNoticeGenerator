AN_Gen v13 GitHub Pages Fix

Why v12 looked broken on GitHub Pages:
- It waited on the external CSV before populating the bank.
- In some GitHub/local-load situations that left the UI blank or stuck at "Loading..."
- Also app.js and CSS filenames were reused, so browser/GitHub cache could keep serving older code.

Fixes:
- The section bank loads immediately from an embedded copy of IncludedSectionContent.csv.
- It then tries to refresh from the external IncludedSectionContent.csv if available.
- CSS and JS are cache-busted:
  - an-gen-v13.css?v=13
  - app-v13.js?v=13

Upload these files to GitHub:
- index.html
- app-v13.js
- an-gen-v13.css
- IncludedSectionContent.csv
- Sparklight_R-purple-rgb.png
- Sparklight_R-Business-purple-rgb.png

You can delete or ignore old app.js / an-gen-v10.css after confirming v13 works.
