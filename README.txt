AN_Gen v12 Order + Links + Attachments

New in v12:
- Manual ordering UI:
  - Edit order numbers per section.
  - Drag-and-drop sections in the included section list.
  - Save Order stores the current manual order in the browser using localStorage.
  - Reset Order returns to CSV order.

- Active hyperlink toggle:
  - When enabled, URLs become clickable <a> links in the web/PDF output.
  - When disabled, URLs remain styled text only.

- PDF attachments:
  - Upload one or more PDF attachments.
  - Attachments are appended to the end of the generated notice.
  - Works for authority letters or required supplemental documents.

Notes:
- Browser printing embedded PDFs can vary by browser. For production, test in Chrome/Edge using:
  Save as PDF, Letter, Margins: None, Scale: 100%, Headers/footers: Off, Background graphics: On.
- The generated notice pages paginate normally; attachment PDFs are appended as full-page embedded objects.
