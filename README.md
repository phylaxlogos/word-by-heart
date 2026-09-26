# Word by Heart

A simple, offline Scripture memorisation app.

**[Download the latest release](https://github.com/phylaxlogos/word-by-heart/releases/latest)**

## Download

Download the ZIP for your computer, extract the whole folder, then run **Start Word by Heart**. You do not need to install Go or create an account.

| Computer | ZIP |
|---|---|
| Mac — Apple silicon (M-series) | [Download](https://github.com/phylaxlogos/word-by-heart/releases/download/v0.2.0/word-by-heart_0.2.0_darwin_arm64.zip) |
| Mac — Intel | [Download](https://github.com/phylaxlogos/word-by-heart/releases/download/v0.2.0/word-by-heart_0.2.0_darwin_amd64.zip) |
| Windows — Intel/AMD (x64) | [Download](https://github.com/phylaxlogos/word-by-heart/releases/download/v0.2.0/word-by-heart_0.2.0_windows_amd64.zip) |
| Windows — ARM | [Download](https://github.com/phylaxlogos/word-by-heart/releases/download/v0.2.0/word-by-heart_0.2.0_windows_arm64.zip) |
| Linux — Intel/AMD (x64) | [Download](https://github.com/phylaxlogos/word-by-heart/releases/download/v0.2.0/word-by-heart_0.2.0_linux_amd64.zip) |
| Linux — ARM64 | [Download](https://github.com/phylaxlogos/word-by-heart/releases/download/v0.2.0/word-by-heart_0.2.0_linux_arm64.zip) |

## Features

- NASB 1995 library with original CrossWire source metadata and copyright notices.
- Chapter practice, memory passage collections, difficulty modes, favourites, and recitation dates.
- Progress saved in your browser and automatically synced to a private database on your computer. No progress is uploaded or bundled with downloads.
- In-app update checks, verified downloads, install/restart, and recovery to the previous app if an update fails.
- **S → Quit Word by Heart** to save and close the local app; the launcher reopens an existing running copy.

Open the app at **http://localhost:8080**. A fresh browser, or one whose site data has been cleared, restores synced progress from the computer database. Wait for the save indicator to confirm the computer copy is saved before clearing browser data. Preserve the extracted `data` folder during manual upgrades; it contains the Bible library.

These are portable, unsigned builds, not notarized installers. Mac launch, browser saving, update and recovery were tested; Windows and Linux packages were cross-compiled and their archives verified, but were not run on those operating systems. Read the included `GETTING-STARTED.md` before first use.

The individual executable assets and `SHA256SUMS` are required by the updater. For a first installation, choose a ZIP above.

[Scripture source and attribution](https://github.com/phylaxlogos/word-by-heart/blob/main/SCRIPTURE-SOURCE.md).

## Updates and privacy

The app checks this repository for new releases. When an update is available, choose **Install update and restart** in the sidebar. The app verifies the download and preserves your library and browser progress. Reading and practice work offline; update checks need an internet connection.

Personal progress, favourites, recitation dates and reading position stay on your computer. Changes save in the browser immediately, then sync to a private SQLite database. Interrupted saves retry automatically. All browsers using the same local app and computer account share this database; there is no account or cloud sync. Theme and sidebar appearance preferences remain browser-specific.

The app creates its personal database on first launch, outside the downloaded app folder, so replacing the app does not replace progress:

| Computer | Personal database |
|---|---|
| Mac | `~/Library/Application Support/Word by Heart/progress.sqlite` |
| Windows | `%AppData%/Word by Heart/progress.sqlite` |
| Linux | `$XDG_CONFIG_HOME/Word by Heart/progress.sqlite`, normally `~/.config/Word by Heart/progress.sqlite` |

To back it up, quit the app and copy that personal database folder. Keep your backup private. Existing v0.1.x browser saves are merged on startup; an older `data/progress.sqlite` is imported when the new personal database is first created, without modifying the old file. No personal progress is included in any release.

This repository contains downloads and release documentation. GitHub’s automatically generated source archives contain this documentation, not an installable app; use the platform ZIPs above.
