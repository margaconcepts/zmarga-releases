# Zmarga downloads

Installers for [Zmarga](https://zmarga.com), an offline ABAP code editor.

**There is no source code here.** This repository exists only to host public
download links. The product is built from a private repository, whose release
workflow pushes the installers here on each tagged release.

## Latest version

These links always resolve to the newest published release, so they are safe to
hard-code on a website or in documentation:

| Platform | Download |
|---|---|
| macOS (Apple silicon & Intel) | [Zmarga-macos-universal.dmg](https://github.com/zmarga-dev/zmarga-releases/releases/latest/download/Zmarga-macos-universal.dmg) |
| Windows 10/11 (x64) | [Zmarga-windows-x64.msi](https://github.com/zmarga-dev/zmarga-releases/releases/latest/download/Zmarga-windows-x64.msi) |
| Linux (x64, AppImage) | [Zmarga-linux-x64.AppImage](https://github.com/zmarga-dev/zmarga-releases/releases/latest/download/Zmarga-linux-x64.AppImage) |
| Linux (x64, Debian/Ubuntu) | [Zmarga-linux-x64.deb](https://github.com/zmarga-dev/zmarga-releases/releases/latest/download/Zmarga-linux-x64.deb) |

The filenames deliberately carry no version number. `latest/download/<name>`
only resolves if the name never changes, so the build renames Tauri's own
versioned output before uploading it. The version is on the release itself.

## These builds are not code-signed

Until a signing certificate is in place, the first launch needs one extra step:

- **macOS** — a double-click is refused. Right-click the app, choose *Open*,
  then confirm. Once only.
- **Windows** — SmartScreen warns. Choose *More info*, then *Run anyway*.

That is what an unsigned installer looks like; it does not indicate anything
wrong with the download. Every release is built in CI from a tagged commit.

## Trial and licensing

The download is the full product. It runs for 30 days of actual use — a day
only counts if you open the app — and a licence key then unlocks it
permanently. Keys are verified on your own machine: Zmarga makes no network
calls, so there is nothing to activate and nothing that phones home.

## Issues

Report problems at <https://zmarga.com>. This repository takes no pull
requests, since it holds no code.
