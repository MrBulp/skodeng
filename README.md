CAMERA SKODENG V5 — recording export diagnostics and iPhone share/save controls.

Preserves V4 camera selection, rotation, mirrors, fullscreen, FIT/FILL, and transparent collapsible overlay.

Install: upload index.html and manifest.webmanifest to the root of github.com/MrBulp/skodeng, replacing previous files; wait for GitHub Pages deployment.

Test: Start camera → Record video → wait 5 seconds → Stop recording → wait for size and playback → SHARE / SAVE TO FILES. If video is empty or canvas.captureStream unsupported, app reports an error.

Browser support caveat: iPhone Safari canvas.captureStream + MediaRecorder compatibility varies; this code is not device-tested. Camera image transformations are baked into video only when canvas recording succeeds. iOS Share sheet may save video to Files rather than Photos.
