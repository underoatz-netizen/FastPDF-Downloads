# Installation

## PikaPDF 0.5.0 for Windows x64

PikaPDF (formerly FastPDF through v0.4.1) is published as a 64-bit Windows application. You can install it using the setup installer or run it directly from the portable archive.

### Download links

- **Installer (Setup, ~5.4 MB):** [PikaPDF-0.5.0-win-x64-Setup.exe](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/download/v0.5.0/PikaPDF-0.5.0-win-x64-Setup.exe)
  `SHA-256: 29c09b1347f2f20a96ad081425c22cda20d6880c5a076833090dddcd649ee1b9`
- **Portable package (~4.1 MB):** [PikaPDF-0.5.0-win-x64.zip](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/download/v0.5.0/PikaPDF-0.5.0-win-x64.zip)
  `SHA-256: 62494f6913657beaec8c33f7a81c710e041a1c1ee39390105203b6f561dc9dbb`
- **Checksum file:** [SHA256SUMS](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/download/v0.5.0/SHA256SUMS)
  `SHA-256: 0901f99ccfaa3910af77c9e0d272827737a4f696e15aed38b3909e01f0ae0710`
- **GitHub release:** [v0.5.0 Release](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/tag/v0.5.0)

### Verification

Before installing or running, verify the integrity of your download in PowerShell:

```powershell
Get-FileHash PikaPDF-0.5.0-win-x64-Setup.exe -Algorithm SHA256
```

Verify that the output hash matches the SHA-256 checksum listed above or in `SHA256SUMS`.

### Installation options

#### Option 1: Setup installer (`.exe`)
1. Download `PikaPDF-0.5.0-win-x64-Setup.exe`.
2. Run the downloaded installer.
3. Follow the setup wizard to complete installation. A fresh install defaults to `Program Files\PikaPDF`.

#### Option 2: Portable package (`.zip`)
1. Download `PikaPDF-0.5.0-win-x64.zip`.
2. Extract the archive to any folder of your choice.
3. Run `FastPDF.exe` directly without installation.

### Upgrading from FastPDF 0.4.1

- The executable inside the ZIP and install folder remains **`FastPDF.exe`**, together with `pdfium.dll` and `licenses/`. Existing shortcuts therefore keep working after the rename to PikaPDF.
- Upgrading over FastPDF 0.4.1 upgrades in place and reuses the existing install directory instead of forcing `Program Files\PikaPDF`.
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
