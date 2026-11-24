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

The filenames deliberately carry no version number. `latest/download/<name>`
only resolves if the name never changes, so the build renames Tauri's own
versioned output before uploading it. The version is on the release itself.

### Windows

Coming soon. The Windows version is published here once its code signing is
in place. Write to <support@zmarga.com> if you would like to hear when.

## Signing

- **macOS**: the app is signed with a Developer ID certificate issued to
  MARGA CONCEPTS PTY LTD and notarised by Apple, so it opens normally with a
  double-click.
- **Windows**: not released yet; it follows once code signing is in place.
  Every release is built in CI from a tagged commit.

## Trial and licensing

The download is the full product. It runs for 30 days of actual use (a day
only counts if you open the app), and a licence key then unlocks it
permanently. Keys are checked on your own machine, so there is nothing to
activate and no account. Zmarga uses the network only when you press Push or
Pull to reach your own git remote.

## Support

Write to <support@zmarga.com> rather than opening an issue here. This
repository holds no code, so it takes no pull requests.
