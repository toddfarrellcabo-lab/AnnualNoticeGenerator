AN_Gen v16 Controls Restore

What happened:
- v15 hid #pageTemplate directly to stop iPhone/Safari from printing it.
- That fixed the blank template page, but it also created a conflict because JavaScript clones #pageTemplate to create generated pages.
- Depending on browser/cache timing, the clone could inherit the hard hidden display behavior, causing sections/columns to look broken.

Fix:
- The template is now wrapped in #templateStore.
- CSS hides #templateStore, not #pageTemplate directly.
- Cloned pages are placed outside #templateStore and forced to display normally.
- Columns and included sections controls remain active.

Upload these files to GitHub:
- index.html
- app-v16.js
- an-gen-v16.css
- IncludedSectionContent.csv
- Sparklight_R-purple-rgb.png
- Sparklight_R-Business-purple-rgb.png

After upload:
- Hard refresh the page.
- On iPhone/Safari, close the tab and reopen if it still shows cached v15 files.
