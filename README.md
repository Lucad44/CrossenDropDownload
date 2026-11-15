<p align="center"><img src="icon.png" width="128" height="128" alt="CrossenDrop"></p>

<h1 align="center">CrossenDrop</h1>

<p align="center"><b>AI-powered AliExpress → eBay (EU) dropshipping for your desktop.</b><br>
Find products, list them on eBay in each site's language, keep stock and prices in sync and get your customers' orders
placed on AliExpress – from one app that keeps your data on your own computer.</p>

## Download – version 1.0.0

| | Download | Requirements |
|---|---|---|
| **macOS** | [**CrossenDrop-1.0.0-macos.zip**](https://github.com/Lucad44/CrossenDropDownload/raw/main/releases/1.0.0/CrossenDrop-1.0.0-macos.zip) (5 MB) | macOS 12 or newer, Apple Silicon or Intel |
| **Linux** | [**CrossenDrop-1.0.0-linux.tar.gz**](https://github.com/Lucad44/CrossenDropDownload/raw/main/releases/1.0.0/CrossenDrop-1.0.0-linux.tar.gz) (5 MB) | Fedora 40 or newer (GNOME) |

You also need a **CrossenDrop license key** (sent with your purchase), an **eBay seller account** and the normal
**AliExpress account** you shop with.

## Install

### macOS
1. Double-click the downloaded zip to unpack it.
2. Open **Terminal** (Applications → Utilities), type `cd ` (with a space), drag the unpacked folder into the window and
   press Return.
3. Run:
   ```bash
   bash install.sh
   ```

No administrator password is needed. CrossenDrop then appears in **Launchpad** and in your Applications folder. If your
Mac has no Python 3.12–3.14 yet, the installer installs it with [Homebrew](https://brew.sh) or tells you to get it from
[python.org](https://www.python.org/downloads/macos/). The first time, macOS may ask whether "python" may use your
keychain – choose **Always Allow**.

### Linux (Fedora)
1. Unpack the download: `tar -xzf CrossenDrop-1.0.0-linux.tar.gz`
2. In a terminal:
   ```bash
   cd CrossenDrop-1.0.0-linux
   bash install.sh
   ```

The installer asks for your password once (system packages) and adds CrossenDrop to your app grid.

### Both
- Add `--with-ollama` to also install the local AI (private and free). You can also use Claude with your own Claude
  subscription – choose it in the app under Settings → AI.
- The first start walks you through the set-up: business details, eBay sites, profit margin, your license key, then
  **Connect eBay** and **Connect AliExpress** (each opens the sign-in page in your web browser).
- A background service keeps your listings, prices and orders up to date, even when the window is closed.

## Update

Download the newest version and run `bash install.sh` again in its folder – your settings and data are kept.

## Uninstall

Run `bash install.sh --uninstall` in the downloaded folder. Your data is kept
(macOS: `~/Library/Application Support/CrossenDrop`, Linux: `~/.local/share/crossendrop`).

## Check your download (optional)

[SHA256SUMS.txt](releases/1.0.0/SHA256SUMS.txt) lists the checksums of the files above:
`shasum -a 256 CrossenDrop-1.0.0-macos.zip` (macOS) or `sha256sum CrossenDrop-1.0.0-linux.tar.gz` (Linux).

---

CrossenDrop is proprietary software. © CrossenDrop. All rights reserved.
eBay allows drop shipping only from wholesale suppliers; you remain responsible for compliance, VAT and customer service.
