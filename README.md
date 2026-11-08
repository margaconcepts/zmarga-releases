# Zmarga downloads

Installers for [Zmarga](https://zmarga.com), an offline ABAP code editor for
macOS and Windows.

**There is no source code here.** This repository exists only to host public
download links. The product is built from a private repository, whose release
workflow pushes the installers here on each tagged release.

## Latest version

These links always resolve to the newest published release, so they are safe to
hard-code on a website or in documentation.

### macOS

| Mac | Download |
|---|---|
| Apple silicon and Intel, one app for both | [Zmarga-macos-universal.dmg](https://github.com/margaconcepts/zmarga-releases/releases/latest/download/Zmarga-macos-universal.dmg) |

Open the `.dmg` and drag Zmarga into Applications.

### Windows

| Windows 10 or 11, x64 | Download |
|---|---|
| Installer for most people | [Zmarga-windows-x64-setup.exe](https://github.com/margaconcepts/zmarga-releases/releases/latest/download/Zmarga-windows-x64-setup.exe) |
| MSI, for IT departments deploying it centrally | [Zmarga-windows-x64.msi](https://github.com/margaconcepts/zmarga-releases/releases/latest/download/Zmarga-windows-x64.msi) |

Zmarga uses Microsoft Edge WebView2, which Windows 11 already includes. On a
Windows 10 machine without it, the installer fetches it from Microsoft.

The filenames deliberately carry no version number. `latest/download/<name>`
only resolves if the name never changes, so the build renames Tauri's own
versioned output before uploading it. The version is on the release itself.

## First launch while builds are unsigned

Signing for both platforms is being set up. Until a release says it is
signed, the first launch needs one extra step:

- **macOS**: a double-click is refused. Right-click the app, choose *Open*,
  then confirm. Once only.
- **Windows**: SmartScreen warns. Choose *More info*, then *Run anyway*.

That is what an unsigned installer looks like. It does not mean anything is
wrong with the download. Every release is built in CI from a tagged commit.

## Trial and licensing

The download is the full product. It runs for 30 days of actual use (a day
only counts if you open the app), and a licence key then unlocks it
permanently. Keys are checked on your own machine, so there is nothing to
activate and no account. Zmarga uses the network only when you press Push or
Pull to reach your own git remote.

## Support

Write to <support@zmarga.com> rather than opening an issue here. This
repository holds no code, so it takes no pull requests.
