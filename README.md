# Simple PDF Tool

A single-file, offline PDF page editor. Merge PDFs, remove or add pages, reorder, rotate, and split a document into several PDFs, all page by page, right in your browser.

**File:** `pdf-tool-standalone.html` (about 2 MB)

---

## Features

- **Scrollable page view:** every page is shown large, one under another, like a normal PDF reader
- **Merge:** add as many PDFs as you like; they join in the order added
- **Remove pages:** one at a time, or select several and delete them together
- **Add pages:** insert another PDF after any page
- **Reorder:** move pages up or down
- **Rotate:** turn any page 90° at a time
- **Split with splitters:** place ✂ markers between pages and get one PDF per section
- **Rename before download:** you choose the file name for every PDF and ZIP
- **Private and offline:** nothing is uploaded; all work happens on your device

---

## Quick start

1. Open `pdf-tool-standalone.html` in Chrome, Edge, Firefox or Safari (double-click it, or open it from your phone's Files app).
2. Tap **+ Add PDF(s)** or drag PDFs onto the page.
3. Edit the pages (see below).
4. Press a download button, name your file, and save.

---

## How to use

### Merge PDFs
Add several PDFs with **+ Add PDF(s)**. Their pages appear in one continuous list. Use ▲ ▼ to rearrange, then press **Download all**.

### Remove pages
- Press **✕** on a page to remove it, or
- Tick the pages (checkbox, or tap the page itself) and press **Delete selected**.

### Add pages
Press **＋** on any page to choose a PDF. Its pages are inserted right after that page.

### Reorder and rotate
- **▲ / ▼** moves a page up or down.
- **↻** rotates a page 90° clockwise each press.

### Split a PDF
1. Between any two pages you'll see a **✂ Split here** strip. Tap it to place a splitter (it turns red). Tap again to remove it.
2. Shortcuts: **✂ After every page** (one PDF per page) and **Remove ✂** (clear all splitters).
3. Press **✂ Split & download (N files)**.
4. Rename each part if you like, then choose:
   - **Download ZIP:** all parts in one ZIP file
   - **Download separately:** each part as its own PDF (your browser may ask to allow multiple downloads)

Example: a 10-page PDF with splitters after pages 3 and 7 gives three files, with pages 1–3, 4–7 and 8–10.

### Download only part of a document
Tick the pages you want and press **Download selected** to get them as one new PDF.

### Naming files
Every download opens a small box with the name filled in. Edit it and confirm. The `.pdf` or `.zip` ending is added automatically, unwanted characters (`/ \ : * ? " < > |`) are removed, and duplicate names get a number (`report-2`).

---

## Sharing the tool

It's one HTML file, so you can:

- Send it by email, WhatsApp, Drive or any chat app. The recipient just opens it in a browser.
- Host it for free (Netlify Drop, GitHub Pages, or any static host) and share the link.

No installation, account, or internet connection is needed.

---

## Privacy

Your PDFs never leave your device. There is no server, tracking, or upload. Closing or refreshing the tab clears everything from the tool's memory.

---

## Known limits

- **Password-protected PDFs** may fail to open. Remove the password first.
- **Very large PDFs** (hundreds of pages or heavy scans) can be slow or use a lot of memory, especially on phones.
- **Bookmarks, form fields and other interactive elements** may not carry over to the new files; page content, images and text do.
- **Refreshing the page** loses your work. Download before closing.
- **On phones**, saving a ZIP or several files may prompt for a location depending on the browser.

---

## Troubleshooting

| Problem | Try this |
|---|---|
| "Could not open file" | The PDF may be damaged or password-protected. |
| Pages show "Loading…" for a long time | Large files render page by page; give it a moment. |
| Download doesn't start | Allow downloads/pop-ups for the page in your browser settings. |
| Only one of several separate downloads saved | Allow "multiple downloads", or use **Download ZIP**. |

---

## Built with

Open-source libraries bundled inside the file:

- [pdf-lib](https://pdf-lib.js.org/) (MIT): builds and edits PDFs
- [PDF.js](https://mozilla.github.io/pdf.js/) (Apache-2.0): draws page previews
- [JSZip](https://stuk.github.io/jszip/) (MIT or GPL-3.0): creates ZIP files
