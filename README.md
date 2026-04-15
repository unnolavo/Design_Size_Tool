# Image Measurement Tool (v1)

A lightweight browser tool to measure real-world lengths inside an uploaded image using a known reference line.

## Implemented in v1
- Single-file app (`index.html`) with embedded CSS + JavaScript.
- Upload image to canvas with auto-fit and preserved aspect ratio.
- Zoom controls (wheel + buttons) and directional nudge pad.
- Draw and edit lines:
  - click-drag-release to create lines
  - drag endpoints to adjust
  - select lines for reference re-assignment
- Reference and scale workflow:
  - enter known value + unit (in/cm)
  - set selected line as reference
  - auto-compute scale (`inches per image pixel`)
- Measurements:
  - non-reference lines display dual-unit lengths (`X.XX in / Y.YY cm`)
- Editing controls:
  - Undo Last
  - Redo Last
  - Clear Lines (keeps reference line)
  - Reset All

## Run locally
1. Open `index.html` directly in Google Chrome.
2. Upload an image.
3. Draw a reference line.
4. Enter known real-world length + unit and click **Set Reference**.
5. Draw additional lines to see real-world measurements.

## Quick manual validation checklist
- [ ] Upload image succeeds and image is centered.
- [ ] Mouse-wheel zoom centers around cursor.
- [ ] Directional nudge pad moves image as expected.
- [ ] First line can be set as reference with inches and centimeters.
- [ ] Additional lines show dual-unit measurements.
- [ ] Endpoint dragging updates line geometry.
- [ ] Undo removes last measurement line.
- [ ] Redo restores last undone measurement line.
- [ ] Clear Lines removes measurement lines but keeps reference line.
- [ ] Reset All clears image, lines, scale, and inputs.

## Known limitations (v1)
- Desktop-first interaction (mouse-centric).
- No persistence/export (session-only).
- Optimized for modern Chrome.
