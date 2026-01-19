# Tap to Place AR with A-Frame

This is a simple example of a "Tap to Place" function for Android AR using the A-Frame library.

## Features

- Uses WebXR for AR on Android devices
- Tap on a surface to place a red cube
- Automatic reticle shows placement position

## Requirements

- Android device with ARCore support
- Modern browser that supports WebXR (Chrome recommended)

## Usage

1. Open the `index.html` file in a browser on your Android device.
2. Allow camera permissions when prompted.
3. Point your camera at a flat surface.
4. A reticle will appear indicating where the object can be placed.
5. Tap the screen to place a red cube at that location.

## Serving the App

For AR to work properly, the page must be served over HTTPS or from localhost.

### Using a Local Server

You can use a simple HTTP server to serve the files locally.

For example, using Python:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000` in your browser.

### Using HTTPS

For production or remote access, serve over HTTPS.

## Troubleshooting

- If AR doesn't start, ensure your device supports ARCore and WebXR.
- Check browser console for errors.
- Make sure you're using a compatible browser (Chrome on Android).

## Dependencies

- A-Frame 1.5.0 (loaded via CDN)