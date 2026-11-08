# Ultra Calendar - Releases

Public downloads for **Ultra Calendar**, a desktop app (Windows and macOS) to allocate work hours
across several agencies with a configurable daily hour cap, per-agency pay rates, and
supervision / unpaid hour tracking. Everything runs locally; data is stored in a JSON file on your machine.

This repository only hosts the installers. Download the latest version from the
[Releases page](../../releases/latest).

## Install

**Windows**: download `Ultra.Calendar.Setup.<version>.exe` and run it. SmartScreen may show a
warning because the installer is not code-signed; choose "More info" and then "Run anyway".

**macOS, Apple Silicon (M1 or newer)**: download `Ultra.Calendar-<version>-arm64.dmg`.
**macOS, Intel**: download `Ultra.Calendar-<version>.dmg`.

Open the DMG and drag Ultra Calendar to Applications. The app is not notarized, so on first launch
right-click the app and choose Open, or run:

```
xattr -dr com.apple.quarantine "/Applications/Ultra Calendar.app"
```

## Features

- Weekly time-grid calendar: drag to add hours, drag blocks to move or resize them, click to edit.
- Daily hour limit across all agencies (default 10h, configurable), optional weekly limit.
- Copy a previous week, all agencies or selected ones.
- Per-agency hourly rate, pay totals per day, week and month.
- Supervision hours and unpaid (overlapped) hours tracked separately.
- Export and import backups.
