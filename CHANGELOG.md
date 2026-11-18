# PikaPDF (formerly FastPDF) changelog

## 0.5.0 — 2026-11-18

PikaPDF 0.5.0 is the PikaPDF branding and feature release for Windows x64 (formerly FastPDF through v0.4.1).

### Download links

- **Release page:** [PikaPDF 0.5.0 on GitHub Releases](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/tag/v0.5.0)
- **Installer (Setup, ~5.4 MB):** [PikaPDF-0.5.0-win-x64-Setup.exe](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/download/v0.5.0/PikaPDF-0.5.0-win-x64-Setup.exe)
- **Portable package (~4.1 MB):** [PikaPDF-0.5.0-win-x64.zip](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/download/v0.5.0/PikaPDF-0.5.0-win-x64.zip)
- **Checksums:** [SHA256SUMS](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/download/v0.5.0/SHA256SUMS)

### Release assets

| Asset | File | Size | SHA-256 |
| --- | --- | --- | --- |
| Installer (Setup) | `PikaPDF-0.5.0-win-x64-Setup.exe` | ~5.4 MB | `29c09b1347f2f20a96ad081425c22cda20d6880c5a076833090dddcd649ee1b9` |
| Portable package | `PikaPDF-0.5.0-win-x64.zip` | ~4.1 MB | `62494f6913657beaec8c33f7a81c710e041a1c1ee39390105203b6f561dc9dbb` |
| Checksums | `SHA256SUMS` | — | `0901f99ccfaa3910af77c9e0d272827737a4f696e15aed38b3909e01f0ae0710` |

### New features & improvements

- **PikaPDF branding and icon:** the application is now named PikaPDF (formerly FastPDF through v0.4.1), with a new product icon.
- **Single-row responsive command bar:** commands are presented in one responsive row with Lucide icons. When the window is narrow, additional commands move into a **More commands** overflow menu.
- **Thumbnails & Bookmarks sidebar (`Ctrl+B`):** page thumbnails and document bookmarks share a sidebar. Unsupported external bookmark actions are safely labelled and never executed.
- **Draw and Highlight:** freehand ink drawing with multiple colours and three stroke widths, plus highlighting of embedded selectable text. Undo and Redo are available with `Ctrl+Z` and `Ctrl+Y`.
- **Save a Copy and unsaved-change protection:** Save a Copy writes a new file and never overwrites existing or source files. Prompts protect unsaved work when closing, opening another document, printing, or exporting PNG images.
- **Enhanced Print dialog:** 1–6 pages per sheet, print preview, colour or monochrome output, duplex printing, Fast/Medium/Detailed quality, By set/By page ordering, and print progress with cancel.
- **Navigation, capture and maintenance commands:** Find (`Ctrl+F`), Go to Page (`Ctrl+G`), Screenshot (`Ctrl+S`), Presentation (`F11`), Rotate pages, PDF to PNG, Image to PDF, Diagnostic panel (`Ctrl+D`), and a manual **Check for Updates** command.
- **Upgrade continuity:** the executable inside the ZIP and install folder remains `FastPDF.exe` (with `pdfium.dll` and `licenses/`) so existing shortcuts keep working.

### Upgrade notes

- A fresh install defaults to `Program Files\PikaPDF`.
- Upgrading over FastPDF 0.4.1 upgrades in place, reuses the existing install directory, and preserves `%LOCALAPPDATA%\FastPDF` settings and recent files.
- Requires Windows 10 or Windows 11, 64-bit (x64), and the Microsoft Visual C++ 2015–2022 Redistributable (x64).
- Binaries and installer packages are unsigned. Windows SmartScreen may display an unknown publisher warning.
- Source code is not included in release packages.
- Verify download integrity using the SHA-256 checksums above or in `SHA256SUMS` before installation or execution.

### Known limitations

- No OCR.
- No Add Text tool.
- Annotation editing is disabled on signed, protected or encrypted PDFs, and on pages that already contain annotations.

## [0.4.1] - 2026-10-26

**Release date:** 2026-10-26.

Quality and hardening release of FastPDF for Windows x64, adding PDF open-duration diagnostics logging.

### Release assets

- **Installer (Setup):** `FastPDF-0.4.1-win-x64-Setup.exe`
  `SHA-256: 9bf2783d18e005578c12295465fda5f967a3f7300392ac99d04cb5e1912c7616`
- **Portable package:** `FastPDF-0.4.1-win-x64.zip`
  `SHA-256: 6f83c88952a491286ee629727c9959b743f727f2df06c613466b5460f8f79456`
- **Checksums:** `SHA256SUMS`
  `SHA-256: 6bc71578dc5c82ad815e0f36926c7be6843a4677f4d1a0a3e5f7b6aed8ccc1ba`
- **Release page:** [FastPDF 0.4.1 on GitHub Releases](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/tag/v0.4.1)

### New features & improvements

- **PDF open-duration diagnostics:** The render worker now measures the whole document-open phase (file mapping, PDFium document open, and page-geometry enumeration) with a steady clock and reports it in the diagnostic log (`Opened: ... (open=N ms)`); previously this field always reported 0 ms. This is a diagnostics/logging improvement only — it does not change how FastPDF opens or renders PDFs and is not a fix for any observed cold-open delay.

### Notes

- Binaries and installer packages are unsigned. Windows SmartScreen may show an unknown publisher warning.
- Source code is not included in release packages.
- Download integrity should be verified using SHA256 checksums before installation or execution.
- This release makes no performance claim: the open-duration number is a diagnostic measurement, not a speedup.

## [0.4.0] - 2026-10-24

Release of FastPDF for Windows x64 introducing Go to Page navigation and render pipeline stability improvements.

### Release assets

- **Installer (Setup):** `FastPDF-0.4.0-win-x64-Setup.exe`
  `SHA-256: 460199db7adec1013786b0ad9d9daf38ee795a79ee599778a5c59d93c952bd45`
- **Portable package:** `FastPDF-0.4.0-win-x64.zip`
  `SHA-256: ed1a16ef1dc2bf404fcbc921856f41a191e2b5a6bec1d0e1726d9a922ddccbb5`
- **Checksums:** `SHA256SUMS`
  `SHA-256: ace327bd80db6a17549a28c6347735d957fed7905d02f78d2722f3a7f3b6c0f7`
- **Release page:** [FastPDF 0.4.0 on GitHub Releases](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/tag/v0.4.0)

### New features & improvements

- **Go to Page (`Ctrl+G`):** Direct navigation dialog allowing instant jumps to any page in the document.
- **Input validation:** Robust 1-based page number parsing and validation with visual error feedback for out-of-range or non-numeric inputs.
- **Cancellation safety:** Viewport render cancellation tokens ensure superseded page renders are cleanly aborted during rapid scrolling or page jumping.
- **Render stability:** Improved background tile rendering resilience and responsiveness during rapid navigation.

### Notes

- Binaries and installer packages are unsigned. Windows SmartScreen may show an unknown publisher warning.
- Source code is not included in release packages.
- Download integrity should be verified using SHA256 checksums before installation or execution.

## [0.3.2] - 2026-10-14

First public release of FastPDF for Windows x64.

### Release assets

- **Installer (Setup):** `FastPDF-0.3.2-win-x64-Setup.exe`
  `SHA-256: f3aea2ac8a683eddbcbe74f25444b3004103f13c31851c962fe114b5fd13b74e`
- **Portable package:** `FastPDF-0.3.2-win-x64.zip`
  `SHA-256: aeaf6af1bcb823325c461faabb6a9fc5a6142c9058a265988a5f06738cd8e51b`
- **Checksums:** `SHA256SUMS`
  `SHA-256: edba88446e2b03e701db895848163f514912e536532d2d90db55d0c34eee2552`
- **Release page:** [FastPDF 0.3.2 on GitHub Releases](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/tag/v0.3.2)

### Features included

- **Document viewing:** Continuous page layout with vertical scrolling, drag-and-drop file opening, command-line file path support, and recent files list.
- **Navigation & zoom:** Fit width (`Ctrl+2`), fit page (`Ctrl+0`), 100% zoom (`Ctrl+1`), zoom controls, and full-screen presentation mode (`F11`).
- **Search:** In-document text search (`Ctrl+F`) with previous/next navigation.
- **Printing:** Print support (`Ctrl+P`).
- **Conversion & export:** Export PDF pages to PNG, convert images to PDF, and capture page region screenshots (`Ctrl+S`).
- **Page rotation:** Rotate current page view and save a rotated copy.
- **Diagnostics:** Optional diagnostic overlay (`Ctrl+D`).

### Notes

- Binaries and installer packages are unsigned. Windows SmartScreen may show an unknown publisher warning.
- Source code is not included in release packages.
- Download integrity should be verified using SHA256 checksums before installation or execution.

## Initial public repository baseline

- Initial public distribution repository structure and documentation.
