SILENT COLORS AR - FIXED LIBRARY VERSION

IMPORTANT FIX:
- Previous page imported Three.js r160, which can conflict with MindAR 1.2.5.
- This page uses Three.js r147 and MindAR 1.2.5 on the same CDN.
- The library is dynamically loaded: failed imports show the real error instead of breaking Start AR.

UPLOAD USING IPHONE:
1. Unzip these files in the iPhone Files app.
2. Open github.com/sammypot/AR.
3. Upload the new index.html to the top/root level and REPLACE existing index.html.
   Also upload alternate.html into the same root folder (optional fallback).
4. Keep the EXISTING targets.mind file at the root; it is not in this ZIP.
5. Keep assets/silent-colors-target.jpg and assets/silent-colors-video.mp4 in assets folder.
6. Optionally upload camera-test.html to the root.
7. Commit the changes, wait for GitHub Pages deployment, then open:
   https://sammypot.github.io/AR/?v=4

Expected repository:
  index.html
  alternate.html   <-- alternative library server if the primary CDN fails
  targets.mind  <-- IMPORTANT: your own compiled painting target file
  camera-test.html
  assets/
    silent-colors-target.jpg
    silent-colors-video.mp4

TROUBLESHOOTING:
- If AR library fails: the page now displays the exact import error.
- Tap Test back camera. If the live room is visible, camera access works.
- Tap Check uploaded files. All three file checks should report OK.
- If camera appears but painting is not detected, regenerate targets.mind from the same JPG using MindAR's official image target compiler.
- In iPhone Safari, automatic sound is blocked until user interaction. Autoplay starts muted.
- The page uses internet for MindAR and Three.js from jsdelivr CDN.

IMPORTANT: This package has been tested for HTML/JS syntax and ZIP integrity,
but physical camera tracking must be tested on the actual phone.

ALTERNATE SERVER:
If the homepage cannot load the AR library, tap Try alternate library server,
or open https://sammypot.github.io/AR/alternate.html.
This requires alternate.html uploaded next to index.html.
