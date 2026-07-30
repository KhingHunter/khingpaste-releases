# KhingPaste releases

The public half of [KhingPaste](https://khingpaste.khingsuite.com), the macOS
clipboard history app. Source lives in a private repository; this one exists so
the shipped app can reach its update feed without a token.

- **`appcast.xml`** — the Sparkle feed. The app fetches it once a day.
- **Releases** — one per version, with the notarised DMG attached. Every
  `<enclosure url>` in the appcast points at one of these assets.

Both must stay reachable to a logged-out request. A private-repo asset URL
returns 404 to Sparkle with no useful error, which is the whole reason this
repository is separate.

Download the current version from
[khingpaste.khingsuite.com](https://khingpaste.khingsuite.com).
