# StageGlass Director — Releases

Public release channel for **StageGlass Director** (macOS). This repository hosts:

- `appcast.xml` — the Sparkle update feed the app reads
  (`SUFeedURL = https://raw.githubusercontent.com/mikecerisano/stageglass-releases/main/appcast.xml`).
- GitHub Releases (tag `director-vX.Y.Z`) carrying the signed, notarized `DirectorApp-X.Y.Z.dmg`,
  referenced from each appcast `<enclosure>`.

Releases are produced from the (private) main `stageglass` repo by
`scripts/release-director.sh`. **Do not edit `appcast.xml` by hand** — the script prepends each
new `<item>`.
