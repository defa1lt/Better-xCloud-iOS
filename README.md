# Better xCloud for iOS (Unofficial)

> An unofficial iOS wrapper for Xbox Cloud Gaming (xCloud) that bundles the **Better xCloud** userscript for a smoother, more console-like experience on iPhone and iPad.

> \[!IMPORTANT]
> **Disclaimer:** This project is **not** affiliated with, endorsed by, or sponsored by Microsoft or Xbox. “Xbox,” “xCloud,” and related marks are trademarks of their respective owners. Use at your own risk.

<p align="left">
  <img alt="iOS 15+" src="https://img.shields.io/badge/iOS-15%2B-blue">
  <img alt="Wrapper" src="https://img.shields.io/badge/WKWebView-Wrapper-lightgrey">
  <img alt="Binary only" src="https://img.shields.io/badge/Distribution-Binary--only-orange">
</p>

**Links**

* Homepage (Better xCloud): [https://better-xcloud.github.io](https://better-xcloud.github.io)
* Userscript repo: [https://github.com/redphx/better-xcloud](https://github.com/redphx/better-xcloud)
* Report **app** issues: open an Issue on this repo’s
* Report **userscript** issues: [https://github.com/redphx/better-xcloud/issues](https://github.com/redphx/better-xcloud/issues)
* Support the script author: [https://ko-fi.com/redphx](https://ko-fi.com/redphx)

---

## Why use the iOS app instead of Safari?

* ✅ All features of the **Better xCloud** userscript (auto-injected)
* ✅ True fullscreen, safe areas ignored
* ✅ Xbox-style preloader (logo + progress bar)
* ✅ Prevents accidental pinch-to-zoom and hides scroll indicators
* ✅ Swipe-to-go-back works like Safari; bottom system gestures are deferred
* ✅ Inline media playback; no forced taps for video/audio
* ✅ Built-in JS/console error logger to help troubleshoot
* ✅ Small, fast, battery-friendly wrapper

> The app doesn’t modify Microsoft’s servers. It loads `xbox.com/play` and enhances it **client-side** using the userscript.

---

## Download & Install

Binary-only distribution. Get the latest **.ipa** from this repository’s **Releases** page.

<details>
<summary><strong>Option A — AltStore (recommended, free)</strong></summary>

1. Install **AltServer** on macOS/Windows.
2. Connect your device and install **AltStore**.
3. On iPhone/iPad: **AltStore → My Apps → + →** select the downloaded **.ipa**.
4. If prompted, trust the developer profile in **Settings → General → VPN & Device Management**.

</details>

<details>
<summary><strong>Option B — Sideloadly (Windows/macOS)</strong></summary>

1. Open **Sideloadly**, connect your device.
2. Drag the **.ipa** in, sign with your Apple ID, and install.

</details>

> \[!NOTE]
> Free Apple IDs require re-signing about every **7 days**. A paid Developer account lasts up to **12 months** per build.

---

## Requirements

* iOS/iPadOS **15.0+**
* An active **Xbox Cloud Gaming**–supported account/region
* Stable internet (5 GHz Wi-Fi recommended; wired gamepad support varies by device)

---

## Features (iOS specifics)

* Preloader waits for **actual UI readiness** (region button / video surface)
* Disables zoom (meta + CSS + gesture blocking) while keeping Safari-style back swipe
* Hides all **scroll indicators** (WebView + in-page elements)
* Defers **bottom system gestures** and auto-hides Home indicator
* Bundled polyfills for `navigator.mediaDevices.*` to avoid site crashes
* Opens `target="_blank"` in the **same view** (PWA-like)
* JS dialogs (`alert`/`confirm`/`prompt`) handled **natively** (e.g., “Quit game” confirm)

---

## Privacy

* The app **does not** collect analytics or personal data.
* Network traffic goes to Microsoft’s Xbox Cloud Gaming domains as part of normal site usage.
* Any telemetry you see in the console (e.g., Application Insights) belongs to **Microsoft’s site**, not this app.

---

## Known Limitations

* Feature availability depends on Microsoft’s site and your region.
* If Microsoft changes the site, some enhancements may temporarily break until the userscript is updated.
* On free certificates (sideloading), the app must be **re-signed periodically**.

---

## Troubleshooting

* **Stuck on loading:** Kill the app and relaunch; ensure network is stable.
* **“Script error” with no stack:** Cross-origin protection in WKWebView; harmless and normal for third-party bundles.
* **No region button / blank UI:** Wait a few seconds; the preloader hides only when the UI is visible. If it persists, try reloading or signing out/in on `xbox.com/play`.
* **Gamepad issues:** Reconnect the controller; if using Bluetooth, toggle it off/on.

---

## Credits

* **Better xCloud** userscript: [https://github.com/redphx/better-xcloud](https://github.com/redphx/better-xcloud) (all credit to the original author and contributors)
* iOS wrapper app by the community. Binary-only distribution.

---

## Legal

This project is provided **“as is,”** without warranty of any kind. By using this app you agree you are responsible for your account and device. **Microsoft/Xbox** are trademarks of Microsoft Corporation. This app is **not** affiliated with or endorsed by Microsoft.

---

## License

* **App binary:** Distributed without source; all rights reserved by the distributor.
* **Userscript:** See its repository for license and terms.

---

If you find this useful, consider ⭐ starring the **Better xCloud** userscript repo or supporting its author.
