# Daymark — Daily Preparation Tracker

**Plan your day, focus on what matters, and build a steady preparation habit.**

Daymark is a free daily planner for desktop, tablet, and mobile. Open it in your browser, or install it on your phone’s home screen for an app-like experience. No account is required.

## Open Daymark

**Start using the app:** [sunilprajapati832.github.io/daymark](https://sunilprajapati832.github.io/daymark/)

You can use Daymark directly in your browser. Installation is optional.

- **Android:** Open the app link in Chrome. Tap **Install** if it appears, or open Chrome’s menu and choose **Install app** or **Add to Home screen**.
- **iPhone:** Open the app link in Safari. Tap **Share → Add to Home Screen**, then tap **Add**. If offered, turn on **Open as Web App**.
- **Computer or tablet:** Open the app link in your browser. Daymark adjusts to your screen size.

For more detail, see the [Android install guide](https://github.com/sunilprajapati832/daymark/blob/main/ANDROID-INSTALL.md). The app is free to use; no subscription or payment is required.

## Preview

### Desktop — Light mode

![Daymark desktop preview, light mode](Preview/daymark1.png)

![Daymark desktop checklist and schedule](Preview/daymark2.png)

### Mobile — Dark mode

<table>
  <tr>
    <td><img src="Preview/Image4.jpeg" alt="Daymark mobile preview 1" width="180"></td>
    <td><img src="Preview/Image3.jpeg" alt="Daymark mobile preview 2" width="180"></td>
    <td><img src="Preview/Image2.jpeg" alt="Daymark mobile preview 3" width="180"></td>
    <td><img src="Preview/Image1.jpeg" alt="Daymark mobile preview 4" width="180"></td>
  </tr>
</table>

## What you can do

- **Plan your checklist:** Add tasks, choose a category, estimate hours, and reorder items with the arrows. Edit or remove tasks whenever you need.
- **Make it personal:** Use a built-in category or choose **Other** and enter your own, such as sleep, play, or exercise.
- **See your day:** Daymark arranges tasks in checklist order and estimates their start times from the start time you choose.
- **Focus with a timer:** Choose a focus session from 30 minutes to 8 hours. The **Break** button switches to a 5-minute break.
- **Track completed days:** The calendar marks a day when every task in that day’s checklist is checked. It shows completed dates and your current consecutive-day streak.
- **Choose your look:** Switch between light and dark mode, and optionally add a display name and profile photo.
- **Get a daily reflection:** The thought changes daily and cycles through 100 original reflections before repeating.

## Quick start

1. Open the app link above.
2. Add your own task, or edit the sample tasks in **Your checklist**.
3. Set an estimated duration and category for each task.
4. Use the arrows to put tasks in your preferred order. **Today’s rhythm** updates to match.
5. Check tasks off as you complete them. Finish every task to mark that date complete in the calendar.

## How daily tracking works

- The calendar checks a date after all tasks on that day’s checklist are complete.
- Completed dates stay in your calendar when the checklist rolls over to a new day.
- A new day starts with the sample checklist. Add or edit tasks for that day as needed.
- The streak counts consecutive completed dates through today, or through yesterday if today is not complete yet.

## Your data and offline use

Daymark saves your tasks, completed dates, profile, and theme in your browser on that device. There are no accounts and no cloud sync, so data is separate on each device. Clearing the browser’s site data can remove your saved information.

After Daymark has loaded once while online, its app shell can reopen offline. The optional Google Fonts may not load without an internet connection; the app uses system fonts as a fallback.

## Feedback and suggestions

If you use Daymark, please share your review, report anything confusing or broken, and suggest features you’d like to see. You can leave feedback through the [GitHub repository](https://github.com/sunilprajapati832/daymark).

## About

Daymark is built with HTML, CSS, and JavaScript by **Sunil Prajapati**.

[Connect with Sunil on LinkedIn](https://www.linkedin.com/in/sunil-prajapati832)




# Daymark — Daily Preparation Tracker

Daymark is a lightweight daily planner for turning preparation into a steady routine. It runs in a browser on desktop and mobile, and can be installed from a secure website address as a Progressive Web App (PWA).

🔗 **App Link**: <br>
[![App Link](https://img.shields.io/badge/App%20Link-daymark-success?style=for-the-badge&logo=google-chrome&logoColor=white)](https://sunilprajapati832.github.io/daymark/)

On Android, open it in Chrome and tap Install if it appears, or choose Install app / Add to Home screen from Chrome’s menu. On iPhone, open it in Safari and choose Share → Add to Home Screen. **Apple’s instructions**


## App Preview
### Desktop View (Light Mode)
![Graph Preview](Preview/daymark1.png)
![Graph Preview](Preview/daymark2.png)

### Mobile View Responsive (Dark Mode)
<table><tr><td><img src="Preview/Image4.jpeg"></td> <td><img src="Preview/Image3.jpeg"></td> <td><img src="Preview/Image2.jpeg"></td> <td><img src="Preview/Image1.jpeg"></td></tr></table>

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

## 👨‍💻 Author

**Sunil Prajapati**<br>
M.E. Graduate | Python & Flask Developer <br>
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Follow%20Me-blue?logo=linkedin&style=for-the-badge)](https://www.linkedin.com/in/sunil-prajapati832)

---

⭐ If you find this project valuable, feel free to star the repository and connect!
