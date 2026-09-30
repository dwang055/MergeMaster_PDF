# MergeMaster PDF

**Merge, arrange and edit PDFs right in your browser. Nothing is ever uploaded.**

MergeMaster PDF is a single-file web app (`MergeMaster_PDF.html`) from **Words That Think · 品词坊 · 以词启思**. Open it, drop in your files, and get a finished PDF. All processing happens on your own device, so it is safe for student work, reports and private documents.

**Try it:** https://dwang055.github.io/MergeMaster_PDF/

---

## Features

### Combine
- Merge any number of PDFs, in any order (drag, or use the ◀ ▶ buttons on touch screens)
- Add images (JPG, PNG, HEIC and more); each becomes an A4 page
- Open password-protected PDFs by entering the password

### Arrange pages
- Page manager with thumbnails for each file
- Delete and restore pages, rotate pages, reorder pages
- Insert one or many blank pages anywhere, including at the start
- Extract selected pages with ranges such as `1-3, 5, 8-`

### Finish
- Page numbers with a custom pattern (e.g. `Page {page} of {total}`) and the option to skip the first pages
- Text watermark, including Chinese, Japanese, Korean and other non-Latin text
- Title and author metadata
- Password-protect the downloaded PDF (AES-256)

### Preview and edit
- Built-in viewer for the merged result
- Add text anywhere on a page, then move it, restyle it and edit it again later
- **OCR text correction** (see notes below): detect the text on a scanned page and fix it in place

### Built for real devices
- Works on desktop, iPad and phone
- Handles large files: pages render lazily, so a 500-page PDF stays responsive
- Correct placement on rotated and landscape pages

---

## How to use

1. Open `MergeMaster_PDF.html` in a modern browser (Chrome, Edge, Safari, Firefox).
2. Add your PDFs and images.
3. Use **Manage pages** on any file to rotate, delete or add blank pages.
4. Choose page numbers, watermark, metadata or a password if you want them.
5. Click **Merge**, check the preview, then **Download**.
6. Optional: click **Edit PDF** to add text or correct OCR text, then **Apply & Save**.

---

## Privacy

Files are read and processed entirely in your browser. There is no server, no account and no tracking. Your documents never leave your device.

## Good to know

- **Internet needed on first load.** The app loads three open-source libraries from a CDN: pdf-lib, PDF.js and Tesseract.js. Your files are never sent to these CDNs. To run fully offline, download the libraries and point the script tags at local copies.
- **OCR needs a full browser.** It uses Web Workers, which some in-app previews block. If OCR reports an error, open the file directly in Chrome, Edge or Safari.
- **OCR accuracy** depends on scan quality. Always check recognised text before saving.
- **Password protection** is applied to the downloaded copy. The preview and editor use an unprotected working copy, so you can keep editing after setting a password.

## Open-source credits

- [pdf-lib](https://github.com/Hopding/pdf-lib) via the [@cantoo/pdf-lib](https://github.com/cantoo-scribe/pdf-lib) fork (merging, editing, encryption)
- [PDF.js](https://github.com/mozilla/pdf.js) (rendering and previews)
- [Tesseract.js](https://github.com/naptha/tesseract.js) (OCR)

## Deploying on GitHub Pages

The app is one HTML file, so there is nothing to build. Put `MergeMaster_PDF.html` in your repository, enable **Settings → Pages**, and it is live at `https://<username>.github.io/<repo>/MergeMaster_PDF.html`.

---

© Daniel Wang · Words That Think. All rights reserved.
