AN_Gen v19 Page Break + Widow Orphan Fix

Built from the stable v18 base.

Fixes added:
- Page-break before a section when it would start with fewer than about 3 body lines.
- Widow/orphan protection checks for paragraphs that would leave only 1-2 lines at the bottom or top of a page.
- CSS widows/orphans hints remain enabled.
- Slight tracking/kerning tightening helps reduce isolated short lines.

Important note:
Web browsers do not provide full InDesign-level typography controls. This gets much closer, but InDesign still has stronger paragraph composer/keep options.

Upload:
- index.html
- app-v19.js
- an-gen-v19.css
- IncludedSectionContent.csv
- Sparklight_R-purple-rgb.png
- Sparklight_R-Business-purple-rgb.png
