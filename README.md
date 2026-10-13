# GISInspector Lite

A small, portable, **Windows** app for construction inspection **Daily** and
**Weekly** reports, plus **Project Edit** and four **inspection logs**. It runs
fully offline.

> This repository holds the **download** only. The source code is not published
> here.

## What it does

- **Project Edit** — add / edit / delete projects: name, DOT agency, contract
  id, allowed days, NTP and target dates, and the reporting week start day.
- **Daily Report** — record the day's inspection (header, arrivals/manpower,
  equipment, the four inspection logs, site observations, remarks, deliveries,
  pay items, next steps) and export a **PDF**.
- **Weekly Report** — roll a chosen week's Daily Reports into a single
  **Weekly PDF**.
- **Inspection logs** — four add / edit / delete logs on the Daily Report page:
  **Concrete Placement**, **Electrical & Conduit**, **Storm Sewer**, and
  **Earthwork**. Each record carries its own date.

All work is stored locally in a `data` folder next to the app. There is no
account, no server, and no internet connection required.

**Export / Import** backs up every project and report to a single JSON file and
restores it back. **Send my work** / **Get latest** can also move work between
two computers through a shared folder (a USB stick, a network share, or a
cloud-synced folder); if both computers changed the same item, the app asks
which version to keep.

## Windows only

This app runs on **Windows**. It is a single `.exe` — no installer, no Python,
and no internet are needed.

## Install

1. Download **`GISInspectorLite-v0.1.0.zip`** from the **Releases** section.
   (This first release, v0.1.0, is published as a **pre-release**.)
2. **Unzip** it into a folder of your choice (for example `C:\GISInspectorLite`).
   Do not run it from inside the zip.
3. Double-click **`GISInspectorLite.exe`** to start.

On first launch the app creates a `data` folder **next to the executable** and
keeps all of your projects and reports there. To move the app to another PC,
copy the whole folder (the `.exe` **and** the `data` folder).

## First-run warning ("unknown publisher")

The app is not code-signed, so Windows may show a **Windows protected your PC**
blue box the first time you run it:

1. Click **More info**.
2. Click **Run anyway**.

## Update

Replace the `.exe`; keep the `data` folder.

1. Close the app (it runs as a single instance — check the taskbar).
2. Delete or rename the old `GISInspectorLite.exe`.
3. Put the new `GISInspectorLite.exe` in the **same folder**.
4. Leave the `data` folder exactly where it is, then start the app again.

Your projects and reports remain. Before updating, it is a good idea to open the
Hub and use **Export** to save a JSON backup.

## Known limitations

- **Arabic text may print reversed** in exported PDFs (the app does not perform
  right-to-left text shaping).
- The app is **unsigned**, so Windows SmartScreen or antivirus software may flag
  it. See the first-run warning above.

## Report a problem

Use the **Issues** tab of this repository. Please include what you did, what you
expected, and what actually happened — and the version shown in the app's status
bar.

**Do not attach real project data** (project names, numbers, PDFs, or database
files) to an Issue.

## License

The software is provided **as is**, without warranty of any kind.
All rights reserved.
