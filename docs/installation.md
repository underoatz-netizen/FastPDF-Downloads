# Installation

## FastPDF 0.4.0 for Windows x64

FastPDF 0.4.0 is published as a 64-bit Windows application. You can install it using the setup installer or run it directly from the portable archive.

### Download links

- **Installer (Setup):** [FastPDF-0.4.0-win-x64-Setup.exe](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/download/v0.4.0/FastPDF-0.4.0-win-x64-Setup.exe)
  `SHA-256: 460199db7adec1013786b0ad9d9daf38ee795a79ee599778a5c59d93c952bd45`
- **Portable package:** [FastPDF-0.4.0-win-x64.zip](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/download/v0.4.0/FastPDF-0.4.0-win-x64.zip)
  `SHA-256: ed1a16ef1dc2bf404fcbc921856f41a191e2b5a6bec1d0e1726d9a922ddccbb5`
- **Checksum file:** [SHA256SUMS](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/download/v0.4.0/SHA256SUMS)
  `SHA-256: ace327bd80db6a17549a28c6347735d957fed7905d02f78d2722f3a7f3b6c0f7`
- **GitHub release:** [v0.4.0 Release](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/tag/v0.4.0)

### Verification

Before installing or running, verify the integrity of your download in PowerShell:

```powershell
Get-FileHash FastPDF-0.4.0-win-x64-Setup.exe -Algorithm SHA256
```

Verify that the output hash matches the SHA-256 checksum listed above or in `SHA256SUMS`.

### Installation options

#### Option 1: Setup installer (`.exe`)
1. Download `FastPDF-0.4.0-win-x64-Setup.exe`.
2. Run the downloaded installer.
3. Follow the setup wizard to complete installation.

#### Option 2: Portable package (`.zip`)
1. Download `FastPDF-0.4.0-win-x64.zip`.
2. Extract the archive to any folder of your choice.
3. Run `FastPDF.exe` directly without installation.

### Security & SmartScreen guidance

The binaries and setup packages are currently **unsigned**. When running the installer or portable executable for the first time, Windows Defender SmartScreen may display an alert dialog ("Windows protected your PC / Unknown publisher").

To proceed safely:
1. Ensure the SHA-256 hash matches the official published checksum above.
2. Click **More info** on the SmartScreen dialog.
3. Click **Run anyway**.

## Where to go next

- Read the [user guide](user-guide.md) for the application's controls and shortcuts.
- Report a problem through the repository's GitHub issue forms; see [SUPPORT.md](../SUPPORT.md).
