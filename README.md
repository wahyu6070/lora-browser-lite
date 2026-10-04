# Lora — a lightweight Android browser

Lora is a small (≈ 2 MB), fast web browser for Android, built with Kotlin, Jetpack Compose
and Material 3 (dynamic color / Material You on Android 12+).

This repository only hosts **release APKs**. Get the latest version from
[**Releases**](https://github.com/wahyu6070/lora-browser-lite/releases/latest).

## Features

- **Tabs** with session restore — your tabs come back even if the phone dies suddenly
- **Can be your default browser** — opens http/https links from other apps
- **Real incognito mode** with its own profile: cookies and site data are wiped when you leave
- **Built-in downloader**
  - confirmation before every download (editable file name, file size, copy link)
  - pause / resume, automatic retry when the connection drops
  - downloads survive the app being closed and can be resumed
  - SHA-256 / MD5 checksum verification
  - **download from a pasted link** — direct files download right away (PixelDrain and
    BuzzHeavier share pages are resolved to the file); web pages open in a new tab
  - **choose where downloads go**: internal storage, an SD card or a USB OTG drive
- **Storage & network at a glance** on the Downloads page — usage of every storage volume
  and live download / upload speed
- **Ad & tracker blocker** (can be turned off)
- **Night mode** rendered by the WebView itself — no white flash, and sites with their own
  dark theme use it
- Bookmarks and history with **pinning** (long-press → pin, copy URL, delete), private sites
  hidden from history
- Search with Google, Bing, DuckDuckGo or Yandex
- User-agent switcher, desktop mode, find in page, view source, translate
- **Per-site camera / microphone / location** permissions, asked only when a site requests them
- HTTP sign-in (e.g. router admin pages) and an error page with a retry button
- Classic (bottom bar) or modern (Chrome-style top bar) layout, adjustable UI scale
- Languages: English, Indonesian, Japanese, Chinese, Russian, Arabic

## Requirements

- Android 8.0 (API 26) or newer
- An up-to-date Android System WebView / Google Chrome (recommended — needed for isolated
  incognito cookies and native night mode)

## Installing

1. Open [Releases](https://github.com/wahyu6070/lora-browser-lite/releases/latest) and download
   `lora-<version>.apk`.
2. Open the file and, if asked, allow "Install unknown apps" for your file manager or browser.
3. Updates install over the previous version — your data is kept.

## Permissions

| Permission | Used for |
|---|---|
| Internet, network state | Browsing |
| Notifications, foreground service | Showing downloads and keeping them running |
| Storage (Android 10 and older only) | Saving downloads to the Download folder |
| Camera, microphone, location | Only asked when a website requests them |

Lora does not use "All files access", ships no trackers, and never sends your browsing history
anywhere.

## Author

Made by [wahyu6070](https://github.com/wahyu6070).

## License

Lora is released under the [MIT License](LICENSE).
