# Mouse Cam

A single-page web app that turns an iPad (or any device with a camera and a modern browser) into a motion-triggered video camera.

**Live:** https://jonasprobst.github.io/mousecam/

## How it works

- Compares downscaled camera frames several times a second; when enough pixels change, it starts recording.
- Keeps recording until no motion has been seen for a set number of seconds (max 2 minutes per clip).
- Clips are stored in the browser's IndexedDB on the device. Nothing is uploaded anywhere.
- Uses the Screen Wake Lock API to keep the screen on, plus a "Darken screen" overlay.

## Use

1. Open the link in Safari on the iPad and allow camera access.
2. Plug the iPad in; set Auto-Lock to Never as a backup.
3. Tap **Start watching**, wave a hand to test (the bar should pass the white line), then leave it.
4. Keep Safari in the foreground — iOS stops the camera when the page is in the background.
5. Review clips on the page and use **Save** to send them to Photos or Files.

## License

MIT
