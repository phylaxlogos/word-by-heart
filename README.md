# Word by Heart

A simple, offline Scripture memorisation app.

**[Download the latest release](https://github.com/phylaxlogos/word-by-heart/releases/latest)**

## Download

Download the installer for your computer. Word by Heart opens in its own desktop window and works offline. You do not need Go, Node, or an account.

| Computer | Installer |
|---|---|
| Mac — Apple silicon (M-series) | [DMG](https://github.com/phylaxlogos/word-by-heart/releases/download/v0.3.0/Word-by-Heart-0.3.0-mac-arm64.dmg) |
| Mac — Intel | [DMG](https://github.com/phylaxlogos/word-by-heart/releases/download/v0.3.0/Word-by-Heart-0.3.0-mac-x64.dmg) |
| Windows — Intel/AMD (x64) | [Setup](https://github.com/phylaxlogos/word-by-heart/releases/download/v0.3.0/Word-by-Heart-0.3.0-win-x64.exe) |
| Windows — ARM64 | [Setup](https://github.com/phylaxlogos/word-by-heart/releases/download/v0.3.0/Word-by-Heart-0.3.0-win-arm64.exe) |
| Linux — Intel/AMD (x64) | [AppImage](https://github.com/phylaxlogos/word-by-heart/releases/download/v0.3.0/Word-by-Heart-0.3.0-linux-x64.AppImage) · [Debian package](https://github.com/phylaxlogos/word-by-heart/releases/download/v0.3.0/Word-by-Heart-0.3.0-linux-x64.deb) |
| Linux — ARM64 | [AppImage](https://github.com/phylaxlogos/word-by-heart/releases/download/v0.3.0/Word-by-Heart-0.3.0-linux-arm64.AppImage) · [Debian package](https://github.com/phylaxlogos/word-by-heart/releases/download/v0.3.0/Word-by-Heart-0.3.0-linux-arm64.deb) |

**Mac:** Open the DMG, drag **Word by Heart** into **Applications**, eject the disk image, and open the installed app. The current Mac app is not Apple Developer ID signed or notarized. If macOS blocks this download, click **Done**, then open **System Settings → Privacy & Security → Open Anyway** for Word by Heart and confirm **Open**. [Apple's instructions](https://support.apple.com/en-us/102445#openanyway).

**Windows:** Run Setup, then open Word by Heart from the Start menu. The current installer is unsigned, so Windows may display a publisher warning.

**Linux:** Mark the AppImage executable and open it, or install the Debian package using your distribution's package installer.

## Features

- NASB 1995 library with original CrossWire source metadata and copyright notices.
- Chapter practice, memory passage collections, difficulty modes, favourites, and recitation dates.
- Progress saved in your browser and automatically synced to a private database on your computer. No progress is uploaded or bundled with downloads.
- A desktop window with a normal app icon, single-instance launch, and save-before-close behavior.
- In-app update checks. Windows Setup and Linux AppImage installations support install/restart; unsigned Mac and Debian installations link to the new download.
- **S → Quit Word by Heart** saves and closes the app. Normal window close and application Quit also save first.

The desktop window restores synced progress from the same computer database used by the previous browser edition. Before switching, wait for the browser edition's save indicator to confirm the computer copy is saved. Reinstalling the app does not replace that database.

Mac automatic desktop updates require Apple signing, which is not configured yet. The installed Mac app offers a download link for new versions. A DMG installer alone does not remove Apple's verification warning.

The installed Apple silicon Mac app has been tested for saving, closing, reopening and recovery. Other installers are built on their native operating-system runners; their graphical installation and runtime behavior have not been manually tested.

The [release assets](https://github.com/phylaxlogos/word-by-heart/releases/tag/v0.3.0) also contain portable browser ZIPs, named `word-by-heart_0.3.0_...zip`. Extract those to a permanent writable folder and run **Start Word by Heart** to use **http://localhost:8080**. Keep the extracted `data` folder when manually upgrading a portable copy. Raw executables and `SHA256SUMS` support its existing updater; they are not the desktop installer.

[Scripture source and attribution](https://github.com/phylaxlogos/word-by-heart/blob/main/SCRIPTURE-SOURCE.md).

## Updates and privacy

The app checks this repository for new releases. Use **Install update and restart** where supported, or download the new installer when offered. Desktop updates replace the installed app; the portable browser edition retains its separate executable updater. Reading and practice work offline; update checks need an internet connection.

Personal progress, favourites, recitation dates and reading position stay on your computer. Changes save in the browser immediately, then sync to a private SQLite database. Interrupted saves retry automatically. All browsers using the same local app and computer account share this database; there is no account or cloud sync. Theme and sidebar appearance preferences remain browser-specific.

The app creates its personal database on first launch, outside the downloaded app folder, so replacing the app does not replace progress:

| Computer | Personal database |
|---|---|
| Mac | `~/Library/Application Support/Word by Heart/progress.sqlite` |
| Windows | `%AppData%/Word by Heart/progress.sqlite` |
| Linux | `$XDG_CONFIG_HOME/Word by Heart/progress.sqlite`, normally `~/.config/Word by Heart/progress.sqlite` |

To back it up, quit the app and copy that personal database folder. Keep your backup private. Existing v0.1.x browser saves are merged on startup; an older `data/progress.sqlite` is imported when the new personal database is first created, without modifying the old file. No personal progress is included in any release.

This repository contains downloads and release documentation. GitHub’s automatically generated source archives contain this documentation, not an installable app; use the installers above.
