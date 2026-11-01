# Install Daymark on Android for free

Daymark is packaged as a Progressive Web App (PWA). It installs from Chrome and runs in its own app window. The app shell is cached for offline opening; checklist data stays in the browser on that device.

## 1. Put the files on a free HTTPS host

Android installation needs a secure `https://` address. One free option is GitHub Pages:

1. Sign in to GitHub and create a **public** repository for Daymark.
2. Upload every file from this folder to the repository's root: `index.html`, `manifest.webmanifest`, `sw.js`, and both icon PNG files.
3. In the repository, open **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, select the `main` branch and `/ (root)`, then save.
4. Wait for GitHub Pages to publish the site. Its address will appear in the Pages settings.

GitHub Pages offers free static hosting for public repositories. The GitHub account and public repository are required; the app itself does not require a paid service.

## 2. Install it on the phone

1. Open the published `https://` address in **Chrome on Android**.
2. Tap **Install** in Daymark if it appears, or open Chrome's menu and choose **Install app** / **Add to Home screen**.
3. Confirm **Install**. Daymark will appear in the app launcher and home screen.

Use the same published address whenever you want to open Daymark in Chrome. Your profile, checklist, and calendar are stored locally in that browser; they do not automatically sync to other devices.
