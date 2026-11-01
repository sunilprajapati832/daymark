# Daymark — Daily Preparation Tracker

Daymark is a lightweight daily planner for turning preparation into a steady routine. It runs in a browser on desktop and mobile, and can be installed from a secure website address as a Progressive Web App (PWA).

🔗 **App Link**: <br>
[![App Link](https://img.shields.io/badge/App%20Link-daymark-success?style=for-the-badge&logo=google-chrome&logoColor=white)](https://sunilprajapati832.github.io/daymark/)

## What it does

- Build a daily checklist, choose a category, and estimate task hours.
- Edit, reorder, complete, and remove checklist tasks.
- Add custom activity categories such as sleep, play, or exercise.
- See the checklist ordered into a daily schedule, with an adjustable start time.
- Use a focus timer with selectable session lengths from 30 minutes to 8 hours, plus a 5-minute break.
- Track daily completion dates and consecutive completed-day streaks in a calendar.
- Set a display name and profile picture, choose a theme, and get a rotating daily reflection.
- Use a responsive layout on desktop, tablet, and phone screens.
- Install the site from Chrome on Android or add it to the iPhone Home Screen from Safari.

## Technology

Daymark uses plain HTML, CSS, and JavaScript. It has no framework, build step, server, account system, or paid app dependency.

- **HTML** contains the page and controls.
- **CSS** provides the visual theme, responsive layouts, and dark mode.
- **JavaScript** handles checklist actions, scheduling, timer, calendar, profile, and saved preferences.
- **Web Storage (`localStorage`)** keeps each person’s tasks, completed dates, streak history, profile, and preferences in that browser.
- **Web app manifest** supplies the installed app name, launch mode, colors, and icons.
- **Service worker** caches the app shell so the site can reopen offline after it has been loaded once.
- **Canvas and FileReader** resize the selected profile picture before saving it locally.

There is no backend or cross-device synchronization. The profile picture and planner data stay in the browser’s local storage. Clearing that browser’s site data can remove them. When online, the page also requests DM Sans and Manrope from Google Fonts; system fonts are used if they are unavailable offline.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | Complete application page, styling, and client-side logic |
| `manifest.webmanifest` | PWA name, appearance, launch URL, and icon declarations |
| `sw.js` | Offline app-shell cache and network behavior |
| `icon-192.png`, `icon-512.png` | Home-screen and launcher icons |
| `ANDROID-INSTALL.md` | GitHub Pages and Android installation walkthrough |

## Run it

You can open `index.html` directly for a quick browser preview. To install the PWA or use offline caching, publish the files over HTTPS (or run them on `localhost`); opening a local `file://` page is not enough for service-worker registration.

### Free publishing with GitHub Pages

1. Create a **public** GitHub repository. GitHub Pages is available for public repositories on GitHub Free.
2. Upload the application files listed above to the repository root and commit them.
3. Open **Settings → Pages**. Select **Deploy from a branch**, choose `main` and `/(root)`, then save.
4. Open the HTTPS site URL GitHub Pages provides. GitHub may take a few minutes to publish the first version.

GitHub’s instructions: [Quickstart for GitHub Pages](https://docs.github.com/en/pages/quickstart).

## Install on a device

- **Android:** Open the HTTPS site in Chrome and choose **Install app** if offered, or use the browser menu’s **Install app** / **Add to Home screen** option.
- **iPhone:** Open the HTTPS site in Safari, tap **Share → Add to Home Screen**, then tap **Add**. If shown, enable **Open as Web App**.

For Android screenshots and details, see [`ANDROID-INSTALL.md`](./ANDROID-INSTALL.md). The PWA needs HTTPS to be installable and register its service worker; the manifest provides its install name and icons. Learn more about [installable PWAs](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps/Guides/Making_PWAs_installable) and [Apple’s Add to Home Screen steps](https://support.apple.com/en-mide/guide/iphone/iph42ab2f3a7/27/ios/27).

## Day tracking rules

- A date is marked complete when every task in that day’s checklist is checked.
- The calendar keeps completed dates as the app rolls the checklist forward to the next day.
- Default tasks reset each new day; completed-day history remains saved.
- The streak counts consecutive completed dates through today, or through yesterday if today is not complete yet.
- The daily reflection rotates through 100 original notes before repeating.

## License

See the repository’s `LICENSE` file for the terms chosen by the owner. If the repository has no license file, the source remains under default copyright restrictions; GitHub’s public-repository terms still allow users to view and fork it.

## Author

**Sunil Prajapati** · [LinkedIn](https://www.linkedin.com/in/sunil-prajapati832)
