# Installation

## PikaPDF 0.5.1 for Windows x64

PikaPDF (formerly FastPDF through v0.4.1) is published as a 64-bit Windows application. You can install it using the setup installer or run it directly from the portable archive.

### Download links

- **Installer (Setup, ~5.4 MB):** [PikaPDF-0.5.1-win-x64-Setup.exe](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/download/v0.5.1/PikaPDF-0.5.1-win-x64-Setup.exe)
  `SHA-256: 39d7e807a1292d080511be8a4ce9ea06922c9a5fe2f15e0687c290f66fee84da`
- **Portable package (~4.1 MB):** [PikaPDF-0.5.1-win-x64.zip](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/download/v0.5.1/PikaPDF-0.5.1-win-x64.zip)
  `SHA-256: 1b912854c6e833de6a71b6b6567f45760d3ea55438e00416ce51e2c0a49b0a6a`
- **Checksum file:** [SHA256SUMS](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/download/v0.5.1/SHA256SUMS)
  `SHA-256: a21a4bb017fff7ead3523f66c295fb6d5f5bda6d1ef0a5cc17647753cd7470d1`
- **GitHub release:** [v0.5.1 Release](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/tag/v0.5.1)

### Verification

Before installing or running, verify the integrity of your download in PowerShell:

```powershell
Get-FileHash PikaPDF-0.5.1-win-x64-Setup.exe -Algorithm SHA256
```

Verify that the output hash matches the SHA-256 checksum listed above or in `SHA256SUMS`.

### Installation options

#### Option 1: Setup installer (`.exe`)
1. Download `PikaPDF-0.5.1-win-x64-Setup.exe`.
2. Run the downloaded installer.
3. Follow the setup wizard to complete installation. A fresh install defaults to `Program Files\PikaPDF`.

#### Option 2: Portable package (`.zip`)
1. Download `PikaPDF-0.5.1-win-x64.zip`.
2. Extract the archive to any folder of your choice.
3. Run `FastPDF.exe` directly without installation.

### Upgrading from FastPDF 0.4.x or PikaPDF 0.5.0

- The executable inside the ZIP and install folder remains **`FastPDF.exe`**, together with `pdfium.dll` and `licenses/`. Existing shortcuts therefore keep working after the rename to PikaPDF.
- Upgrading over FastPDF 0.4.x or PikaPDF 0.5.0 upgrades in place and reuses the existing install directory instead of forcing `Program Files\PikaPDF`.
- Your settings and recent-files list in `%LOCALAPPDATA%\FastPDF` are preserved during an in-place upgrade.

### System requirements

- Windows 10 or Windows 11, 64-bit (x64).
- Microsoft Visual C++ 2015–2022 Redistributable (x64).

### Security & SmartScreen guidance

The binaries and setup packages are currently **unsigned**. When running the installer or portable executable for the first time, Windows Defender SmartScreen may display an alert dialog ("Windows protected your PC / Unknown publisher").

To proceed safely:
1. Ensure the SHA-256 hash matches the official published checksum above.
2. Click **More info** on the SmartScreen dialog.
3. Click **Run anyway**.

## Where to go next

- Read the [user guide](user-guide.md) for the application's controls and shortcuts.
- Report a problem through the repository's GitHub issue forms; see [SUPPORT.md](../SUPPORT.md).
