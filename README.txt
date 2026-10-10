SILENT COLORS - NEW iPHONE-FRIENDLIER AR BUILD
==============================================
For GitHub repository: https://github.com/sammypot/AR
Live site after publishing: https://sammypot.github.io/AR/

IMPORTANT
- This package replaces the old A-Frame page with the official MindARThree
  rendering workflow. It shows real camera video behind a transparent 3D
  overlay, starts your video when the painting is found, pauses on loss, and
  provides camera diagnostics if Safari shows a black screen.
- We cannot run a physical iPhone camera/image-target test from here.
- Keep your existing targets.mind file in the ROOT of your GitHub repository.
  This package does NOT contain targets.mind. You must use the .mind file
  compiled from the exact painting image assets/silent-colors-target.jpg.

SIMPLEST UPDATE ON IPHONE
1. Download index.html separately from the assistant response.
2. In Safari, open github.com/sammypot/AR.
3. In the repository ROOT, tap Add file > Upload files. Select index.html.
   Upload it to the ROOT, not inside assets. Commit the update.
4. If GitHub says the file already exists, choose to replace/overwrite it.
   If uploading on iPhone makes a duplicate filename, ensure the final
   ROOT filename is EXACTLY index.html (not index (1).html).
5. Your repository should have:
   index.html
   targets.mind
   assets/silent-colors-target.jpg
   assets/silent-colors-video.mp4
6. Open Settings > Pages and keep main, / (root), and HTTPS.
7. Wait 1-3 minutes; open https://sammypot.github.io/AR/?v=3
   The ?v=3 avoids reusing a stale cached HTML page.
8. Tap Start AR, allow camera, point phone at the original painting.

IF THE CAMERA IS STILL BLACK
- Tap 'Test camera' on the AR screen, or open
  https://sammypot.github.io/AR/camera-test.html
  (if you uploaded the included camera-test.html too).
- If the plain camera test shows the room, the camera works and the issue
  is AR rendering or the phone/browser GPU.
- If the plain camera test is also black, check Safari permission,
  iPhone camera use by other apps, and try reloading.
- Screenshot the STATUS/DIAGNOSTICS text and send it for further diagnosis.

IF CAMERA WORKS BUT VIDEO DOES NOT APPEAR
- Ensure targets.mind is compiled using EXACTLY the target JPG.
- Ensure .mind is in ROOT, while MP4/JPG are inside assets/.
- Move camera slowly and include most of the artwork in the frame.
- If iPhone stops video autoplay, tap the visible Play video button.
- Tap Enable sound after the image is detected to hear the soundtrack.

PRODUCTION NOTES
- Uses Three.js 0.160 + mind-ar 1.2.5 from public CDNs.
- Hosted on GitHub Pages, no paid license needed.
- Secure HTTPS and internet access needed to load the page.
- Video is 720x884 H.264 MP4 with fast-start metadata; ~7.8 MB.
- To use a QR code, the included PNG encodes the GitHub Pages URL.
