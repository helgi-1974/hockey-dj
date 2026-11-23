# Hockey DJ — GitHub Pages PWA

## Publish without a Mac
1. Create a public GitHub repository named `hockey-dj`.
2. Upload the five web files (`index.html`, `app.js`, `sw.js`, `manifest.webmanifest`, `icon.svg`) to the repository root (not the containing folder).
3. In GitHub, go to **Settings → Pages**, choose **Deploy from a branch**, select `main` and `/ (root)`, and save.
4. Wait for GitHub Pages to publish, then visit `https://YOUR-USERNAME.github.io/hockey-dj/` on your iPhone in Safari.
5. Tap **Share → Add to Home Screen**.

## Use
- Import songs from the iPhone Files app. Files are stored in the browser's IndexedDB, locally on that device. They do not sync between phones.
- Tap any song to play. The next song starts when it ends.
- Tap GOAL, POWER PLAY or a last-minute button for a cue. Import custom recordings in Settings to replace built-in cues.
- STOP ALL stops audio controlled by this app, not other apps such as Apple Music.
- iOS may evict website data when storage is constrained; keep original audio files and reimport if necessary.
- Built-in announcements use speech synthesis, which can depend on available device voices and connectivity. For dependable offline use, import prerecorded announcements.
- Test sound and Bluetooth/PA routing before use. Keep screen awake during games.

## Limitations
- Apple Music subscription library and DRM downloads cannot be directly accessed by a GitHub Pages web app using file input. MusicKit on the Web is a separate future integration requiring Apple developer configuration and potentially a backend for secure token handling.
- Goal song is not bundled. Import audio you are permitted to use.
- Generated fanfare is original oscillator-based sound; announcer voice uses browser text-to-speech rather than a prerecorded voice actor.
- No guarantee of uninterrupted background playback or mixing with external audio apps on iOS.
- This is an initial prototype and has not been tested on an iPhone.
