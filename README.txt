AN_Gen v14 Print Blank Fix

Why you were getting blank pages:
1. The generated page was set to exactly 11in tall.
2. Chrome/Edge print headers/footers or default print margins add extra printable-space requirements.
3. That made the bottom footer spill onto a new sheet, creating mostly blank pages between content pages.
4. The uploaded PDF showed browser headers/footers were on: URL/date/Page text appeared on every page.

Fixes in v14:
- Print page height reduced from 11in to 10.72in so the internal footer no longer spills to a blank browser page.
- Print margins are forced to zero where CSS can control it.
- CSS/JS filenames are cache-busted:
  - an-gen-v14.css?v=14
  - app-v14.js?v=14

Still recommended in Chrome/Edge Print:
- Destination: Save as PDF
- Paper: Letter
- Margins: None
- Headers and footers: OFF
- Background graphics: ON
- Scale: 100%

Upload these files to GitHub:
- index.html
- app-v14.js
- an-gen-v14.css
- IncludedSectionContent.csv
- Sparklight_R-purple-rgb.png
- Sparklight_R-Business-purple-rgb.png
