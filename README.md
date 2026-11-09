# Ultra Calendar - Releases

Public downloads for **Ultra Calendar**, a desktop app (Windows and macOS) to allocate work hours
across several agencies with a configurable daily hour cap, per-agency pay rates, and
supervision / unpaid hour tracking. Everything runs locally; data is stored in a JSON file on your machine.

This repository only hosts the installers. Download the latest version from the
[Releases page](../../releases/latest).

## Install

**Windows**: download `Ultra-Calendar-Setup-<version>.exe` and run it. SmartScreen may show a
warning because the installer is not code-signed; choose "More info" and then "Run anyway".

**macOS, Apple Silicon (M1 or newer)**: download `Ultra-Calendar-<version>-arm64.dmg`.
**macOS, Intel**: download `Ultra-Calendar-<version>-x64.dmg`.

Open the DMG and drag Ultra Calendar to Applications. The app is not notarized by Apple yet, so the first
launch is blocked with a message that macOS cannot verify it. This is a one-time step per Mac:

1. Double-click Ultra Calendar once and dismiss the dialog.
2. Open System Settings > Privacy & Security, scroll down to the Security section, and click **Open Anyway**
   next to Ultra Calendar. Confirm with your password or Touch ID.
3. Launch the app again. It opens normally from now on.

(On macOS 15 and later, the old right-click > Open shortcut no longer bypasses this check.)

Alternative from a terminal:

```
xattr -dr com.apple.quarantine "/Applications/Ultra Calendar.app"
```

## Updates

From version 0.2.4 the app checks this repository for a newer release when it starts and every 4 hours
(Settings > Updates has the switch and a "Check now" button).

- Windows: the new installer downloads in the background; click "Restart to update" when it is ready.
- macOS: the app shows a "Download" button that opens the release page. It cannot replace itself until the
  app is signed with an Apple Developer certificate.

The .zip, .blockmap and .yml files attached to each release are used by that check; you do not need them.

## Features

- Weekly time-grid calendar: drag to add hours, drag blocks to move or resize them, click to edit.
- Daily hour limit across all agencies (default 10h, configurable), optional weekly limit.
- Copy a previous week, all agencies or selected ones.
- Per-agency hourly rate, pay totals per day, week and month.
- Supervision hours and unpaid (overlapped) hours tracked separately.
- Export and import backups.
