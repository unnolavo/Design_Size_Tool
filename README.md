# Image Measurement Tool (v1 in progress)

A lightweight browser tool to measure real-world lengths inside an uploaded image.

## Current progress
- Stage 0/1 complete:
  - Single-file app (`index.html`) with embedded CSS and JavaScript.
  - Image upload + canvas rendering.
  - Auto-fit image to canvas while preserving aspect ratio.
  - Basic zoom in/out controls.
  - Status/hint text and placeholder controls for upcoming stages.

## Run locally
1. Open `index.html` directly in Google Chrome.
2. Upload an image.
3. Use Zoom + / Zoom - to inspect fit.

## Next stages
- Draw lines by click-drag-release.
- Set reference line + known value (in/cm).
- Measure additional lines in both inches and centimeters.
- Undo last line, clear lines, reset all.
