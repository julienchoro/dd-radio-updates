# DD Radio updates

Small public update feed used by the DD Radio TestFlight build.

The app reads `update.json` on launch. If `latestBuild` is greater than the
installed app build number, it shows a simple update message with a TestFlight
button.

Example:

```json
{
  "latestBuild": 4,
  "message": "Une nouvelle version de DD Radio est disponible sur TestFlight.",
  "updateURL": "https://testflight.apple.com"
}
```

Keep `latestBuild` equal to the currently available TestFlight build. Do not set
it to a future build before that build is actually available.
