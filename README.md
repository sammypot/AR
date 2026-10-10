# Silent Colors AR — GitHub Pages package

This folder is ready to upload to a **public GitHub repository** and publish with **GitHub Pages**.

## What it does
1. Visitor opens the GitHub Pages link.
2. Taps **Start AR** and allows camera access.
3. Points the camera at `assets/silent-colors-target.jpg`.
4. The video in `assets/silent-colors-video.mp4` appears over the artwork and plays.
5. When the artwork is lost, playback pauses.

## Upload to GitHub
1. Create a new **Public** repository, for example `silent-colors-ar`.
2. Click **Add file → Upload files**.
3. Upload **index.html** and the entire **assets** folder, preserving the folder structure.
4. Commit the files.
5. Go to **Settings → Pages**.
6. Under **Build and deployment**, choose **Deploy from a branch**.
7. Select **main** and **/(root)**, then Save.
8. Wait a few minutes. GitHub will show the live HTTPS URL.

## Important
- Internet is required because MindAR and A-Frame are loaded from CDNs and GitHub Pages hosts the site.
- Test on a physical phone using Safari (iPhone) or Chrome (Android).
- Allow camera permission.
- Keep the full target image visible in good lighting when first detecting it.
- The first page load compiles the target image in the browser, so it may take several seconds depending on the phone.

## After publishing
Send the GitHub Pages URL back to ChatGPT and ask for a QR code. The QR should point to that exact live URL.
