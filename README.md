# PikaPDF for Windows

PikaPDF (formerly **FastPDF** through v0.4.1) is a Windows PDF utility from
**OZ Lab** for opening, reading, searching, presenting, printing and capturing
PDFs, and for converting PDFs to PNG and images to PDF.

[ไทย](README.th.md)

PikaPDF 0.5.1 (released 2026-11-22) is available for 64-bit Windows. You can download the installer or portable package directly from GitHub Releases.

## Downloads (v0.5.1)

- **Release page:** [PikaPDF 0.5.1 Release](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/tag/v0.5.1)
- **Installer (Setup, ~5.4 MB):** [PikaPDF-0.5.1-win-x64-Setup.exe](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/download/v0.5.1/PikaPDF-0.5.1-win-x64-Setup.exe)
  `SHA-256: 39d7e807a1292d080511be8a4ce9ea06922c9a5fe2f15e0687c290f66fee84da`
- **Portable package (~4.1 MB):** [PikaPDF-0.5.1-win-x64.zip](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/download/v0.5.1/PikaPDF-0.5.1-win-x64.zip)
  `SHA-256: 1b912854c6e833de6a71b6b6567f45760d3ea55438e00416ce51e2c0a49b0a6a`
- **Checksums:** [SHA256SUMS](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/download/v0.5.1/SHA256SUMS)
  `SHA-256: a21a4bb017fff7ead3523f66c295fb6d5f5bda6d1ef0a5cc17647753cd7470d1`

> **Note on security & SmartScreen:** Binaries and installer packages in this release are unsigned. When opening the downloaded file, Windows Defender SmartScreen may display a prompt ("Windows protected your PC"). Click **More info** and then **Run anyway** if you choose to proceed. Always verify file checksums with `Get-FileHash` before running.

## What PikaPDF does

PikaPDF is a native Windows application. Key capabilities in v0.5.1:

- **System-Aware Theme** — automatically follows Windows Light/Dark app
  settings (`AppsUseLightTheme`) and High Contrast mode at startup and live on
  system theme changes (`WM_SETTINGCHANGE` / `WM_THEMECHANGED`), updating the
  DWM title bar, Explorer controls, command bar, sidebar, Find panel, and
  notification toasts without re-rendering cached PDF pages or altering
  Presentation Mode.

- **Open and view** — open a PDF, drag a single file onto the window, or pass a
  file path on the command line.
- **Command bar** — a single-row responsive command bar with Lucide icons and a
  **More commands** overflow menu for narrower windows.
- **Read and navigate** — continuous page layout with zoom, fit width, fit page,
  Go to Page (`Ctrl+G`), Find (`Ctrl+F`), page rotation, and a full-screen
  presentation mode (`F11`).
- **Thumbnails & Bookmarks sidebar** (`Ctrl+B`) — page thumbnails and document
  bookmarks in one sidebar. Unsupported external bookmark actions are safely
  labelled and never executed.
- **Draw and Highlight** — freehand ink drawing with multiple colours and three
  stroke widths, plus highlighting of embedded selectable text, with Undo/Redo
  (`Ctrl+Z` / `Ctrl+Y`).
- **Save a Copy and unsaved-change protection** — saves to a new copy, never
  overwriting existing or source files, and prompts before actions that could
  discard unsaved changes (close, open, print and PNG export).
- **Enhanced Print dialog** — 1–6 pages per sheet, print preview,
  colour/monochrome, duplex, Fast/Medium/Detailed quality, By set/By page
  ordering, and progress with cancel.
- **Convert** — PDF to PNG and image to PDF.
- **Screenshots** — select a region of a page and copy it to the clipboard
  (`Ctrl+S`).
- **Diagnostics and updates** — diagnostic panel (`Ctrl+D`) and a manual
  **Check for Updates** command.

## Upgrading from FastPDF

- The executable inside the ZIP and install folder remains **`FastPDF.exe`**
  (alongside `pdfium.dll` and `licenses/`), so existing shortcuts keep working.
- A fresh install defaults to `Program Files\PikaPDF`.
- Upgrading over FastPDF 0.4.1 or PikaPDF 0.5.0 upgrades in place, reuses the
  existing install directory, and preserves your `%LOCALAPPDATA%\FastPDF`
  settings and recent files.

## Requirements and known notes

- Windows 10 or Windows 11, 64-bit (x64).
- Microsoft Visual C++ 2015–2022 Redistributable (x64).
- Binaries are unsigned, so SmartScreen may warn on first run.
- No OCR.
- No Add Text tool.
- Annotation editing is disabled on signed, protected or encrypted PDFs, and on
  pages that already contain annotations.

## Verification

To verify download integrity, compare the SHA-256 hash in PowerShell:

```powershell
Get-FileHash PikaPDF-0.5.1-win-x64-Setup.exe -Algorithm SHA256
```

Compare the output hash with the published values listed above or in `SHA256SUMS`.

## Documentation

- [Installation guide](docs/installation.md)
- [User guide](docs/user-guide.md)
- [Changelog](CHANGELOG.md)
- [Support & donations](SUPPORT.md)

## Help and feedback

Please use this repository's GitHub issue forms:

- [Report a bug or request a feature](https://github.com/underoatz-netizen/FastPDF-Downloads/issues/new/choose)

Do not include documents, personal data, credentials, license keys or other
sensitive information in an issue.

## Copyright

PikaPDF (formerly FastPDF) is proprietary software. Copyright (c) 2026 OZ Lab.
All rights reserved. See [COPYRIGHT.md](COPYRIGHT.md).
