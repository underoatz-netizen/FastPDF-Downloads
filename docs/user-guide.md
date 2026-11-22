# PikaPDF user guide

A concise reference for PikaPDF (formerly FastPDF) on Windows. It reflects the
application's implemented controls in PikaPDF 0.5.1. For setup details, see the
[installation guide](installation.md).

## Opening a document

- **More commands > Open…** or **Ctrl+O** — open a PDF.
- **Drag and drop** a single PDF file onto the window.
- Pass a file path on the command line when launching the application.
- **More commands > Recent Files** — reopen or clear a recently opened document.
- If the current document has unsaved changes, PikaPDF prompts before opening
  another document.

## Command bar

- PikaPDF uses a single-row responsive command bar with Lucide icons.
- When the window is too narrow to show every command, the remaining commands
  move into the **More commands** overflow menu.
- Frequently used commands include Open, Find, Go to Page, Print, Draw,
  Highlight, Rotate, Screenshot, Presentation and the sidebar toggle.

## Thumbnails & Bookmarks sidebar

- **Ctrl+B** — show or hide the sidebar.
- **Thumbnails** — preview pages and jump to a page by clicking its thumbnail.
- **Bookmarks** — navigate the document's bookmark tree.
- Unsupported external bookmark actions are safely labelled and are never
  executed.

## Viewing and navigation

- **Continuous page layout** with a vertical scrollbar.
- **Go to Page (`Ctrl+G`)** — jump directly to any page number.
- **Mouse wheel** — scroll the document.
- **Ctrl + mouse wheel** — zoom in or out, centred on the cursor.
- **Ctrl+1** — 100% zoom. **Ctrl+2** — fit width. **Ctrl+0** — fit page.
- **Zoom In / Zoom Out** buttons on the command bar (or in **More commands**) — step the zoom level.
- **Page Down / Page Up** — next / previous page.
- **Home / End** — first / last page.
- **Arrow Up / Arrow Down** — small scroll step.
- **Space / Shift+Space** — page down / page up.
- **Double-click a page** — fit page.
- **Drag a page** — pan when the document is larger than the viewport.
- **Rotate left / Rotate right** — rotate the current page for viewing.

## Find

- **Ctrl+F** — show the Find panel.
- Use the panel's previous / next result controls to move between matches.
- Close the panel with its close button or with **Esc**.

## Presentation mode

- **F11** — enter presentation mode; **F11** or **Esc** — leave it.
- While presenting: **Right / Down / Space** — next page, **Left / Up** —
  previous page, **Home / End** — first / last page, left click — next page,
  mouse wheel — previous / next page.

## Draw and Highlight

- **Draw** — freehand ink drawing with multiple colours and three stroke
  widths.
- **Highlight** — highlight embedded selectable text in the PDF.
- **Undo (`Ctrl+Z`)** and **Redo (`Ctrl+Y`)** — step backward or forward through
  annotation changes.
- Use **Save a Copy** to write the annotated result to a new file. PikaPDF does
  not overwrite the original or any existing file.
- Annotation editing is disabled on signed, protected or encrypted PDFs, and on
  pages that already contain annotations.
- There is no **Add Text** tool.

## Save a Copy and unsaved changes

- **Save a Copy** saves the current document, including annotations, to a new
  file that you name. Existing files and the original source file are never
  overwritten.
- PikaPDF prompts when unsaved changes could be lost — for example when closing
  the document or application, opening another document, printing, or exporting
  PNG images.
- Choose **Cancel** in the prompt to return to the document and save your work
  with Save a Copy.

## Printing

- **Ctrl+P**, the print button, or **More commands > Print…** — open the enhanced Print dialog.
- Print options include:
  - **1–6 pages per sheet**
  - **Print preview**
  - **Colour or monochrome** output
  - **Duplex** printing
  - **Fast / Medium / Detailed** quality
  - **By set / By page** ordering
- The dialog shows print progress and provides a **Cancel** button.
- If the document has unsaved changes, PikaPDF prompts before printing.

## Convert

- **More commands > PDF to PNG…** — export pages as PNG images. If the document has unsaved changes, PikaPDF prompts first.
- **More commands > Image to PDF…** — build a PDF from image files.

## Screenshots

- **Ctrl+S** or the screenshot button (also in **More commands**) — enter screenshot mode.
- Drag a rectangular region over a page. The selected region is copied to the
  clipboard, and the toast offers to save it as a PNG image.
- (`Ctrl+S` is screenshot capture, not document save.)
- **Esc** — cancel screenshot mode.

## Page rotation

- **Rotate left / Rotate right** in the command bar rotate the current page for
  viewing.
- Use **More commands > Save a Copy…** (or **Save Rotated Copy…** for rotation-only changes) to save a new copy of the document.

## Diagnostics and updates

- **Ctrl+D** — toggle the diagnostic panel.
- Use **More commands > Check for Updates** to manually check for a newer release.

## Theme

- **System-Aware Theme** — PikaPDF automatically adapts to your Windows Light/Dark app setting (`AppsUseLightTheme`) and High Contrast window luminance at startup and live when system theme settings change (`WM_SETTINGCHANGE` / `WM_THEMECHANGED`).
- The DWM title bar, Explorer scrollbars/controls, single-row command bar, Thumbnails & Bookmarks sidebar, Find panel, and notification toasts follow the active system theme without re-rendering cached PDF pages.
- PDF page rendering, Presentation Mode's black background, search highlights, and annotation brushes remain unchanged.

## Keyboard shortcuts

| Action | Shortcut |
| --- | --- |
| Open a PDF | `Ctrl+O` |
| Find | `Ctrl+F` |
| Go to Page | `Ctrl+G` |
| Show/hide sidebar | `Ctrl+B` |
| Print | `Ctrl+P` |
| Screenshot | `Ctrl+S` |
| Presentation mode | `F11` (leave with `F11` or `Esc`) |
| Undo | `Ctrl+Z` |
| Redo | `Ctrl+Y` |
| 100% zoom | `Ctrl+1` |
| Fit width | `Ctrl+2` |
| Fit page | `Ctrl+0` |
| Diagnostic panel | `Ctrl+D` |
| Next / previous page | `Page Down` / `Page Up` |
| First / last page | `Home` / `End` |
| Small scroll step | `Arrow Up` / `Arrow Down` |
| Page down / page up | `Space` / `Shift+Space` |
| Close dialog, panel or mode | `Esc` |

## Known limitations

- **No OCR** — scanned documents are not converted to searchable text.
- **No Add Text tool** — text cannot be added to a PDF.
- **Annotation editing is disabled** on signed, protected or encrypted PDFs,
  and on pages that already contain annotations.
- **Unsigned binaries** — Windows SmartScreen may warn on first run.
- **Save a Copy only** — PikaPDF does not overwrite the original or existing
  files.

## Getting help and reporting a problem

- Help and issue reporting use this repository's GitHub issue forms:
  [open an issue](https://github.com/underoatz-netizen/FastPDF-Downloads/issues/new/choose).
- When reporting a problem, describe what you did and what happened. **Do not
  attach or paste documents, personal data, credentials, license keys or other
  sensitive information.** A short description and the steps are enough.

<!-- Release metadata: PikaPDF v0.5.1 (2026-11-22)
     Installer SHA-256: 39d7e807a1292d080511be8a4ce9ea06922c9a5fe2f15e0687c290f66fee84da
     Portable SHA-256: 1b912854c6e833de6a71b6b6567f45760d3ea55438e00416ce51e2c0a49b0a6a
     SHA256SUMS SHA-256: a21a4bb017fff7ead3523f66c295fb6d5f5bda6d1ef0a5cc17647753cd7470d1
-->
