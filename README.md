<div align="center">

<img src="https://raw.githubusercontent.com/jubayarbd/nonoise-extension/main/assets/icons/icon128.png" alt="NoNoise Logo" width="96" height="96" />

# NoNoise
### Distraction Blocker & Focus Tool

**Free. Forever. No tracking. No accounts. Runs 100% locally.**

[![Chrome Web Store](https://img.shields.io/chrome-web-store/v/didbpbpmbnbmenjgkbcglghijldljoei?label=Chrome&logo=googlechrome&logoColor=white&color=4285F4)](https://chromewebstore.google.com/detail/nonoise/didbpbpmbnbmenjgkbcglghijldljoei)
[![Firefox Add-ons](https://img.shields.io/amo/v/nonoise?label=Firefox&logo=firefox&logoColor=white&color=FF7139)](https://addons.mozilla.org/en-US/firefox/addon/nonoise/)
[![Chrome Users](https://img.shields.io/chrome-web-store/users/didbpbpmbnbmenjgkbcglghijldljoei?label=Users&color=34A853)](https://chromewebstore.google.com/detail/nonoise/didbpbpmbnbmenjgkbcglghijldljoei)
[![Chrome Rating](https://img.shields.io/chrome-web-store/rating/didbpbpmbnbmenjgkbcglghijldljoei?label=Rating&color=FBBC04)](https://chromewebstore.google.com/detail/nonoise/didbpbpmbnbmenjgkbcglghijldljoei)

<a href="https://chromewebstore.google.com/detail/nonoise/didbpbpmbnbmenjgkbcglghijldljoei">
  <img src="https://img.shields.io/badge/Install%20on-Chrome-4285F4?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Install on Chrome" />
</a>
&nbsp;
<a href="https://addons.mozilla.org/en-US/firefox/addon/nonoise/">
  <img src="https://img.shields.io/badge/Install%20on-Firefox-FF7139?style=for-the-badge&logo=firefox&logoColor=white" alt="Install on Firefox" />
</a>

---

*Built from personal frustration with doom-scrolling. Given to the world for free.*

> **Note:** NoNoise is a closed-source extension. This repository is the public home for documentation, feature roadmap, bug reports, and community discussion. The extension is available on the Chrome Web Store and Firefox Add-ons — no installation from source needed.

</div>

---

## The Problem

YouTube Shorts. Facebook Reels. Instagram Explore. Twitter trending. The modern web is engineered to steal your attention — and it's working.

Every existing tool either blocks the entire site (too extreme), costs money, or does just one thing. NoNoise is different: it's **surgical**. Hide the addictive parts, keep the useful parts, and build real focus habits on top — all for free, forever.

---

## Features

### 🚫 Smart Distraction Blocking

Hide the most addictive parts of the web without blocking the whole site. The popup **automatically shows only the controls relevant to your current tab** — no clutter.

| Platform | What you can hide |
|---|---|
| **YouTube** | Home Feed, Shorts, Recommended sidebar, Comments, Entertainment videos |
| **Facebook** | Reels, Stories, News Feed, Notifications badge |
| **Instagram** | Reels, Explore, Feed |
| **Twitter / X** | Timeline, Trending section |

---

### ⏱️ Pomodoro Focus Timer

A full focus timer built into the dashboard — not bolted on as an afterthought.

- Set custom work and break durations
- **Forced Focus Enforcement** — when a session starts, automatically enables grayscale and blocks images/videos across the web
- **Popup Mini-Timer** — a compact bar synced in real time inside the extension popup
- Shows real-world end time (*"Ends at 7:50 PM"*) so you can plan around it
- Survives browser sleep — built on `chrome.alarms` for Manifest V3 reliability

---

### 📊 Productivity Dashboard

Track what you've protected.

- **Total Distractions Blocked** — every hidden feed, every suppressed Reel, counted
- **Total Focus Time** — cumulative deep work hours across all sessions
- **Total Focus Sessions** — completed Pomodoro cycles
- Reset stats anytime with a confirmation modal

---

### 🌿 Mindful Nudge (Scroll Protection)

Breaks the doomscrolling loop without being aggressive.

- Monitors **active scroll time** — not just time-on-page
- Timer pauses when you stop and resumes when you start again (real scroll time, not reading time)
- After your set limit, shows a gentle glassmorphism toast at the bottom of the screen
- Auto-dismisses after 8 seconds; grace period prevents immediate re-nudging
- Configurable time limit (5–30 minutes)

---

### 🎨 Global Visual Filters

- **Grayscale Mode** — strips dopamine-inducing color from any website
- **Image Blocking** — hides all images globally for distraction-free reading
- **Video Blocking** — removes all video embeds globally
- **Visual Exceptions** — whitelist specific domains (e.g. `quran.com`, `github.com`) to bypass all filters

When media is blocked, the empty space can show **Focus Text Overlays** — choose between Motivational Quotes or Islamic Dhikr.

---

### 🕌 Islam Zone

A dedicated space for spiritual productivity — a feature you won't find in any other extension.

- **Durud Reminder** — plays gentle audio at your chosen interval (every 5, 10, 15, 30, or 60 minutes)
- 9 local audio tracks with a Random Shuffle option
- **Smart Audio Queue** — Durud reminders and Pomodoro alerts never overlap or cut each other off
- Shows next scheduled play time
- Works on both Chrome and Firefox

---

### ⚡ Universal Video Speed Controller

- Floating speed bubble on any video, any website
- Range: 0.25x to 3.0x
- Keyboard shortcuts: **Alt + ↑** / **Alt + ↓**

---

### 🔒 Advanced Protection

- **Strict Mode** — locks the Master Switch so you can't impulsively disable the extension during weak moments
- **Smart Blocklist** — block any website permanently or temporarily, with optional GitHub Gist sync
- **Blocked Page** — custom page explaining why a site is blocked, to reinforce your intent

---

## Privacy

NoNoise is built on one promise: **your data never leaves your device.**

| What NoNoise does | What NoNoise never does |
|---|---|
| ✅ Stores all settings locally | ❌ No analytics or telemetry |
| ✅ Runs 100% in your browser | ❌ No user accounts or sign-up |
| ✅ Works fully offline | ❌ No external servers |
| ✅ Optional Gist sync (your own Gist, your control) | ❌ No data collection of any kind |

---

## Installation

**Chrome, Brave, Edge, or any Chromium browser:**
[→ Install from Chrome Web Store](https://chromewebstore.google.com/detail/nonoise/didbpbpmbnbmenjgkbcglghijldljoei)

**Firefox (Desktop & Android):**
[→ Install from Firefox Add-ons](https://addons.mozilla.org/en-US/firefox/addon/nonoise/)

---

## Permissions

NoNoise requests only what it needs — nothing more.

| Permission | Why it's needed |
|---|---|
| `activeTab` | Read the current tab's URL to show context-aware controls |
| `storage` | Save your settings locally on your device |
| `alarms` | Power the Pomodoro timer and Durud reminders reliably |
| `offscreen` *(Chrome only)* | Play Durud audio in the background without a visible page |

NoNoise does **not** request `history`, `bookmarks`, `cookies`, `identity`, or any permission that touches your personal data.

---

## How NoNoise Compares

| Feature | **NoNoise** | StayFocusd | DF YouTube | News Feed Eradicator | LeechBlock |
|---|---|---|---|---|---|
| YouTube Shorts blocking | ✅ | ❌ | ✅ | ❌ | ❌ |
| Facebook / Instagram controls | ✅ | ❌ | ❌ | ✅ (FB only) | ❌ |
| Pomodoro Focus Timer | ✅ | ❌ | ❌ | ❌ | ❌ |
| Mindful Scroll Nudge | ✅ | ❌ | ❌ | ❌ | ❌ |
| Grayscale / Visual Filters | ✅ | ❌ | ❌ | ❌ | ❌ |
| Islam Zone / Dhikr reminders | ✅ | ❌ | ❌ | ❌ | ❌ |
| Video Speed Controller | ✅ | ❌ | ❌ | ❌ | ❌ |
| Firefox + Android support | ✅ | ❌ | ❌ | ✅ | ✅ |
| Completely free | ✅ | ✅ | ✅ | ✅ | ✅ |
| No tracking / no accounts | ✅ | ❌ | ✅ | ✅ | ✅ |

---

## Roadmap

| Feature | Status |
|---|---|
| Schedule Mode (auto-block during set hours/days) | 🗓️ Planned |
| Custom New Tab page (clock + daily goal) | 🗓️ Planned |
| Per-site daily time limits | 🗓️ Planned |
| Dark Mode injection (force dark on any site) | 🗓️ Planned |
| Hide like/view counts (YouTube, Instagram) | 🗓️ Planned |
| Panic Lock (lock all settings for a set duration) | 🗓️ Planned |
| Max tab limiter | 🗓️ Planned |
| Reading Mode (strip articles to text only) | 🗓️ Planned |

Have a feature idea? [Open a request →](https://github.com/jubayarbd/nonoise-extension/issues/new)

---

## Bug Reports & Feedback

NoNoise is built and maintained by one person. Every bug report and review genuinely makes a difference.

- 🐛 **Found a bug?** [Open an issue](https://github.com/jubayarbd/nonoise-extension/issues/new)
- 💡 **Have an idea?** [Request a feature](https://github.com/jubayarbd/nonoise-extension/issues/new)
- 📧 **Direct contact:** [jubayer.hussain250@gmail.com](mailto:jubayer.hussain250@gmail.com)
- ⭐ **Enjoying NoNoise?** A review on the [Chrome Web Store](https://chromewebstore.google.com/detail/nonoise/didbpbpmbnbmenjgkbcglghijldljoei) or [Firefox Add-ons](https://addons.mozilla.org/en-US/firefox/addon/nonoise/) is the single best way to support a solo developer.

---

<div align="center">

Built with patience and a lot of ☕ by **[Jubayer Hossain](https://jubayarbd.github.io/portfolio)**

*If NoNoise gives you back even one hour of focused work, it was worth building.*

**[⭐ Star this repo](https://github.com/jubayarbd/nonoise) · [🐛 Report a bug](https://github.com/jubayarbd/nonoise-extension/issues) · [Install on Chrome](https://chromewebstore.google.com/detail/nonoise/didbpbpmbnbmenjgkbcglghijldljoei) · [Install on Firefox](https://addons.mozilla.org/en-US/firefox/addon/nonoise/)**

</div>
