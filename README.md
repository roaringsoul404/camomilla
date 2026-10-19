# Camomilla

A free menu bar app for macOS that converts files while you drag them.
Drag a file, hold Shift, and drop it on a petal: Camomilla writes the copy next to the original.

This repository holds the releases of the app. The code of the app is not published here.

## Download

[Download Camomilla.dmg](https://github.com/roaringsoul404/camomilla/releases/latest/download/Camomilla.dmg)

1. Open the disk image.
2. Drag Camomilla to Applications.
3. Open Camomilla from Applications, not from the disk image: only that copy updates itself.

Or paste this in Terminal:

```sh
curl -fsSL https://camomilla.app/install.sh | sh
```

The command downloads the latest version from this page, checks its SHA-256 sum, copies Camomilla to Applications and opens it.
It doesn’t use sudo. macOS opens Camomilla without the steps below. [Read the script](https://camomilla.app/install.sh).

Requirements: a Mac with Apple silicon and macOS 14 or later.

## The first time you open it

Camomilla is not notarized by Apple, so the first time macOS stops the copy you downloaded from the browser. You allow it once:

1. Open Camomilla from Applications. When macOS says it can’t be opened, click Done.
2. Open System Settings, then Privacy & Security, and scroll down to Security.
3. Next to the line about Camomilla, click Open Anyway.
4. Confirm with Touch ID or your password. Camomilla opens, and macOS won’t ask again, not even after updates.

On macOS 14 Sonoma, Control-click Camomilla in Applications, choose Open, then click Open.

## License

Camomilla is free for personal use and for work, under the terms in [LICENSE](LICENSE).
Do not publish the app anywhere else: share the link to this page.

## Source code of the included programs

Camomilla includes FFmpeg and LAME, which are under the GNU LGPL.
Each release has their source code, with the script that builds them, in the file
`Camomilla-<version>-included-programs-source.zip`. `SHA256SUMS.txt` lists the checksums of the files of the release.

## Problems

To report a problem, write to support@camomilla.app. Say what you dragged, which petal you chose and which version of macOS you use.
Camomilla is a free project: there is no promise of an answer or of a fix.
