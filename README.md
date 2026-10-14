# GISInspector Lite

A small, offline **Windows** app for construction inspection **Daily** and
**Weekly** reports, plus **Project Edit** and four **inspection logs**.

This repository is for **downloads only**. The source code is not published
here.

## Download (v0.1.1)

Two downloads are available. Pick the one that fits:

| Download | Recommended for | Instructions |
| --- | --- | --- |
| **[GISInspectorLite-Setup-v0.1.1.exe](https://github.com/gis1948/GISInspectorLite/releases/download/v0.1.1/GISInspectorLite-Setup-v0.1.1.exe)** | Most users | Double-click the installer, click **Next/Finish**. It installs for **your user account only** (no admin rights). |
| **[GISInspectorLite-Portable-v0.1.1.zip](https://github.com/gis1948/GISInspectorLite/releases/download/v0.1.1/GISInspectorLite-Portable-v0.1.1.zip)** | USB stick or portable use | Unzip anywhere (e.g. USB) and run GISInspectorLite.exe. No installation needed. |

**Windows only (64-bit).**

## First run

The app is **unsigned**, so Windows SmartScreen may show *"Windows protected your PC"* on first run. If it does:
1. Click **More info**
2. Click **Run anyway**

Some antivirus tools may also warn about an unsigned download. This is a false positive in many cases; see the [SIGNING_NOTES.md](https://github.com/gis1948/GISInspectorLite-source/blob/master/SIGNING_NOTES.md) in the source repo for details (source repo is private).

## Where your data is stored

- **Installer:** Documents\GISInspectorLite
- **Portable:** data\ next to GISInspectorLite.exe

The app shows the exact folder in **About** (top-right of the Hub). 
**Uninstalling does not delete your data.** If you uninstall the installer, Documents\GISInspectorLite remains on your PC.

## Updating

- **Installer:** Run a newer Setup EXE to upgrade in place. Your data in Documents\GISInspectorLite is kept.
- **Portable:** Unzip a newer zip into the same folder, but **keep the existing data\ folder**.

## Known limitations

- **Arabic text order:** Arabic may print reversed in PDFs. Full bidirectional text support is not yet implemented.
- **Unsigned app:** The app is unsigned, so Windows SmartScreen and some antivirus programs may flag it on first run. Use "More info → Run anyway" if needed.
- **Windows only.** No macOS/Linux build.

## Report a problem

Use the [Issues tab](https://github.com/gis1948/GISInspectorLite/issues). **Do not attach real project data to an Issue.** A description of what happened, steps to reproduce, any error messages, and (if possible) the pp.log from your data folder is usually enough.

**Software provided as is, all rights reserved.**
