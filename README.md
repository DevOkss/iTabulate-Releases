# iTabulate Releases

Download page and release archive for **iTabulate**, the live tabulation host
for judged events.

Judges and tabulators do not need the source code. This repository exists so
that installers can be downloaded publicly and so the desktop app can check for
updates without depending on any private repository.

## Download

Grab the installer for your platform from the
[Releases page](https://github.com/DevOkss/iTabulate-Releases/releases/latest).

| Platform | File | Install |
| --- | --- | --- |
| Windows 64-bit | `iTabulate-Setup-<version>-x64.exe` | Run the installer, choose a folder |
| Windows 64-bit (no install) | `iTabulate-Portable-<version>-x64.exe` | Run it from anywhere, e.g. a USB stick |
| macOS (Apple silicon) | `iTabulate-<version>-arm64.dmg` | Open the disk image, drag to Applications |
| macOS (Intel) | `iTabulate-<version>-x64.dmg` | Open the disk image, drag to Applications |

## Running an event

1. Start iTabulate on the host computer. It starts its own server, so nothing
   else needs to be installed or launched.
2. The Events screen shows the address for this network, for example
   `http://192.168.1.20:3000`. It is also printed to the console when the app
   starts.
3. Connect every phone, tablet or laptop to the **same Wi-Fi**.
4. Each judge opens that address in a browser, enters the event code shown on
   the event's Join panel, and scores from there. No installation on judge
   devices.

Internet access is not required. Events, scores and results are stored in a
SQLite database in the host's own user-data folder, so installing an update
never affects them.

## Automatic updates

The app checks this repository for a newer version shortly after it opens. The
download happens in the background and the new version is installed the next
time the app is closed, so an update never interrupts live scoring. If the
venue has no internet access, the check is skipped silently.

## Older versions

Every published version is kept, so you can reinstall an earlier build if a
new one misbehaves on your machine.
