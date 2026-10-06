# Readwise Sync releases

Public macOS downloads and the signed Sparkle update feed for Readwise Sync.

- Website: https://scarvy.github.io/readwise-sync-releases/
- Downloads: https://github.com/Scarvy/readwise-sync-releases/releases
- Update feed: https://scarvy.github.io/readwise-sync-releases/appcast.xml

The feed will be available after the first signed release is published.

## Publishing

Build and sign releases in the application source repository. Upload the notarized DMG
and SHA-256 checksum to a release here, tagged `vVERSION`. Only after the release is
publicly downloadable, copy its generated `appcast.xml` into this repository's root
and push to `main`. GitHub Pages serves the file unchanged; `.nojekyll` disables
site processing. Never edit a signed feed by hand.

The source code, private signing keys, and local credentials do not belong in this
repository. Users install the first update-enabled version manually, then use the
app's update settings.
