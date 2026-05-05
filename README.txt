AN_Gen v17 Keep-with-Next + Tracking

New behavior:
- If a new section would start near the bottom of a page with less than about 3 lines of body text available, the section jumps to the next page.
- Adds subtle CSS tracking/kerning:
  --body-tracking: -0.004em
  --tight-tracking: -0.006em
  --heading-tracking: -0.01em

Notes:
- CSS widows/orphans is not fully reliable across browsers, especially mobile Safari.
- The JavaScript keep-with-next rule is the reliable part.
- Kerning/tracking can reduce widows/orphans but cannot eliminate every case like InDesign can.

Upload these files:
- index.html
- app-v17.js
- an-gen-v17.css
- IncludedSectionContent.csv
- logo PNGs
