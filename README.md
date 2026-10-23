# FastPDF for Windows

FastPDF is a Windows PDF utility from **OZ Lab** for opening, reading,
searching, presenting, printing and capturing PDFs, and for converting PDFs to
PNG and images to PDF.

[ไทย](README.th.md)

FastPDF 0.3.2 is available for 64-bit Windows. You can download the installer or portable package directly from GitHub Releases.

## Downloads (v0.3.2)

- **Release page:** [FastPDF 0.3.2 Release](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/tag/v0.3.2)
- **Installer (Setup):** [FastPDF-0.3.2-win-x64-Setup.exe](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/download/v0.3.2/FastPDF-0.3.2-win-x64-Setup.exe)
  `SHA-256: f3aea2ac8a683eddbcbe74f25444b3004103f13c31851c962fe114b5fd13b74e`
- **Portable package:** [FastPDF-0.3.2-win-x64.zip](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/download/v0.3.2/FastPDF-0.3.2-win-x64.zip)
  `SHA-256: aeaf6af1bcb823325c461faabb6a9fc5a6142c9058a265988a5f06738cd8e51b`
- **Checksums:** [SHA256SUMS](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/download/v0.3.2/SHA256SUMS)
  `SHA-256: edba88446e2b03e701db895848163f514912e536532d2d90db55d0c34eee2552`

> **Note on security & SmartScreen:** Binaries and installer packages in this release are unsigned. When opening the downloaded file, Windows Defender SmartScreen may display a prompt ("Windows protected your PC"). Click **More info** and then **Run anyway** if you choose to proceed. Always verify file checksums with `Get-FileHash` before running.

## What FastPDF does

FastPDF is a native Windows application. Key capabilities in v0.3.2:

- **Open and view** — open a PDF, drag a single file onto the window, or pass a
  file path on the command line.
- **Read and navigate** — continuous page layout with zoom, fit width, fit page,
  and a full-screen presentation mode.
- **Search** — in-document text search.
- **Print** — print the current document.
- **Convert** — PDF to PNG and image to PDF.
- **Screenshots** — select a region of a page and copy it to the clipboard.
- **Page rotation** — rotate the current page and save a rotated copy.

## Verification

To verify download integrity, you can compare the SHA-256 hash in PowerShell:

```powershell
Get-FileHash FastPDF-0.3.2-win-x64-Setup.exe -Algorithm SHA256
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

FastPDF is proprietary software. Copyright (c) 2026 OZ Lab. All rights
reserved. See [COPYRIGHT.md](COPYRIGHT.md).
