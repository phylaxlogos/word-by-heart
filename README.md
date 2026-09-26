# Word by Heart

A simple, offline Scripture memorisation app.

**[Download the latest release](https://github.com/phylaxlogos/word-by-heart/releases/latest)**

## Download

Download the ZIP for your computer, extract the whole folder, then run **Start Word by Heart**. You do not need to install Go or create an account.

| Computer | ZIP |
|---|---|
| Mac — Apple silicon (M-series) | [Download](https://github.com/phylaxlogos/word-by-heart/releases/download/v0.1.1/word-by-heart_0.1.1_darwin_arm64.zip) |
| Mac — Intel | [Download](https://github.com/phylaxlogos/word-by-heart/releases/download/v0.1.1/word-by-heart_0.1.1_darwin_amd64.zip) |
| Windows — Intel/AMD (x64) | [Download](https://github.com/phylaxlogos/word-by-heart/releases/download/v0.1.1/word-by-heart_0.1.1_windows_amd64.zip) |
| Windows — ARM | [Download](https://github.com/phylaxlogos/word-by-heart/releases/download/v0.1.1/word-by-heart_0.1.1_windows_arm64.zip) |
| Linux — Intel/AMD (x64) | [Download](https://github.com/phylaxlogos/word-by-heart/releases/download/v0.1.1/word-by-heart_0.1.1_linux_amd64.zip) |
| Linux — ARM64 | [Download](https://github.com/phylaxlogos/word-by-heart/releases/download/v0.1.1/word-by-heart_0.1.1_linux_arm64.zip) |

## Features

- NASB 1995 library with original CrossWire source metadata and copyright notices.
- Chapter practice, memory passage collections, difficulty modes, favourites, and recitation dates.
- Progress saved only in your browser. No progress is uploaded or bundled with downloads.
- In-app update checks, verified downloads, install/restart, and recovery to the previous app if an update fails.
- **S → Quit Word by Heart** to save and close the local app; the launcher reopens an existing running copy.

Always use **http://localhost:8080** in the same browser profile to keep your saved progress. Clearing site data clears that browser's progress. Preserve the extracted `data` folder during manual upgrades.

These are portable, unsigned builds, not notarized installers. Mac launch, browser saving, update and recovery were tested; Windows and Linux packages were cross-compiled and their archives verified, but were not run on those operating systems. Read the included `GETTING-STARTED.md` before first use.

The individual executable assets and `SHA256SUMS` are required by the updater. For a first installation, choose a ZIP above.

[Scripture source and attribution](https://github.com/phylaxlogos/word-by-heart/blob/main/SCRIPTURE-SOURCE.md).

## Updates and privacy

The app checks this repository for new releases. When an update is available, choose **Install update and restart** in the sidebar. The app verifies the download and preserves your library and browser progress. Reading and practice work offline; update checks need an internet connection.

Personal progress, favourites, and recitation dates stay in your browser’s local storage. There is no progress account, cloud sync, or progress database. Switching browser profiles, addresses, or ports uses separate storage. No personal progress is included in any release.

This repository contains downloads and release documentation. GitHub’s automatically generated source archives contain this documentation, not an installable app; use the platform ZIPs above.
