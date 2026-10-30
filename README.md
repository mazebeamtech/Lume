<div align="center">

<img src="assets/logo.png" width="128" height="128" alt="Lume logo">

# Lume

**Browse the future.**

A calm, fast browser for Mac, written in Swift and powered by WebKit. Vertical tabs, separate spaces, one command bar, built-in ad blocking and Chrome extensions.

[Download](../../releases) · [Features](#features) · [Shortcuts](#keyboard-shortcuts) · [What's new](#whats-new-in-030)

</div>

---

> **Lume is in beta.** It's ready for everyday browsing, but expect the occasional bug. Feedback is welcome: open an issue and tell us what you ran into.

## About

Lume is a native macOS web browser written in **Swift** with **SwiftUI**. It renders pages with **WebKit**, the same engine that powers Safari, so sites work as you'd expect while the app stays light and feels at home on a Mac.

## Features

### Tabs and spaces
- **Vertical tabs:** your tabs live in a sidebar, where titles stay readable even with a lot open.
- **Spaces:** keep work, school and home apart. Each space has its own tabs, colours, search engine and separate logins. Swipe sideways on the sidebar to switch.
- **Folders and pinned tabs:** group tabs into folders, and pin the sites you live in to a grid at the top. Drag tabs to reorder them or move them between spaces.
- **Split view:** show two tabs side by side.
- **Peek:** shift-click a link to preview it in a floating card without leaving the page.
- **Sleeping tabs:** tabs you haven't used for a while free their memory and wake up right where you left them.
- **Media controls:** see which tab is playing sound, mute it from the sidebar, or control it from the mini player.

### Getting around
- **Command bar:** search, open a site, jump to a tab, or find something in your bookmarks and history from one place. You can also run actions like "Clear browsing data" by typing their name.
- **Start page:** new tabs open to your favourites and recently visited sites.
- **Find on page**, **reader mode** for distraction-free articles, and **picture in picture** for videos.
- **Library:** downloads, history, bookmarks, passwords, extensions, spaces and Boosts, all behind one button in the sidebar.

### Privacy and security
- **Lume Shield:** a built-in ad and tracker blocker (EasyList and EasyPrivacy) that stops them before they load. Turn it off for any site with one click.
- **HTTPS upgrades:** Lume switches sites to a secure connection whenever they support one, with an optional HTTPS-Only mode.
- **Per-site permissions:** camera, microphone, location and pop-ups are asked once per site, and you can change them from the lock in the address bar.
- **Pop-up blocking**, a **"Not Secure" warning** on insecure sites, and **Clear Browsing Data** for any time range.
- **Private tabs:** an incognito tab that leaves nothing behind.

### Passwords
- Saves logins to your Mac's **Keychain**, and only fills them on the site they belong to, after **Touch ID**.
- Suggests strong passwords, and imports passwords from Chrome, Safari, Firefox or 1Password (CSV).

### Extensions and customisation
- **Chrome extensions:** install from the Chrome Web Store with **Add to Lume**, then pin them to the toolbar or keep them in the extensions menu. Most Manifest V3 extensions work.
- **Boosts:** restyle or tweak any site with your own CSS and JavaScript.
- **Your shortcuts:** change any keyboard shortcut in Settings.
- **Light and dark:** follows your Mac, or pick a side.

### Your data
- **Import** bookmarks and history from Chrome, Arc, Brave, Edge, Vivaldi, Opera, Firefox, Zen or Safari.
- **Backup and restore** your spaces, tabs, bookmarks, history and settings to a single file.
- Set Lume as your **default browser**.

## What's new in 0.3.0

- Chrome extension support, with installs straight from the Chrome Web Store.
- Lume Shield ad and tracker blocking, HTTPS upgrades, pop-up blocking and per-site permissions.
- The new Library, folders, split view, Peek, reader mode, sleeping tabs and Boosts.
- A smarter command bar with suggestions, history, bookmarks and actions.
- Safer passwords with Touch ID, a password generator and CSV import.
- A redesigned setup that helps you pick an ad blocker.
- Fixes for file uploads, sign-in pop-ups, fullscreen video, site alerts, and sites that only use `http://`.

## Requirements

| | |
|---|---|
| **Operating system** | macOS 15.4 (Sequoia) or later |

## Install

1. Download the latest `Lume.dmg` from [Releases](../../releases).
2. Open it and drag **Lume.app** into your **Applications** folder.
3. Open Lume.

### "Lume can't be opened"

Lume isn't notarized by Apple, so macOS blocks it the first time you open it. To allow it:

1. Try to open Lume once. macOS shows a message that it can't be opened. Click **Done**.
2. Open **System Settings → Privacy & Security**.
3. Scroll down to the message about Lume and click **Open Anyway**, then confirm with your password or Touch ID.

You only need to do this once. On macOS 15 and later, right-click → Open no longer skips this step.

If you're comfortable with Terminal, this does the same thing:

```bash
xattr -cr /Applications/Lume.app
```

### Updates

From 0.4.0 on, Lume updates itself. It checks once a day, or choose **Lume → Check for Updates…**. Updates are signed and install without the step above. You can turn automatic checks off in **Settings → General → Updates**. If you're on 0.3.0 or earlier, download 0.4.0 by hand once.

## Keyboard shortcuts

These are the defaults. You can change any of them in **Settings → Shortcuts**.

| Shortcut | Action |
|---|---|
| ⌘T | New tab or search |
| ⌘L | Open location |
| ⌘W | Close tab |
| ⇧⌘T | Reopen closed tab |
| ⌃⇥ and ⌃⇧⇥ | Next and previous tab |
| ⌘1 to ⌘9 | Go to a tab |
| ⌘N | New window |
| ⇧⌘N | New incognito tab |
| ⌘R | Reload |
| ⌘[ and ⌘] | Back and forward |
| ⌘F | Find on page |
| ⇧⌘R | Reader mode |
| ⌃⌘P | Picture in picture |
| ⌘S | Show or hide the sidebar |
| ⇧⌘L | Open the Library |
| ⌘D | Bookmark this page |
| ⌘Y | History |
| ⌘J | Downloads |
| ⇧⌘C | Copy page address |
| ⇧⌘⌫ | Clear browsing data |
| Shift-click a link | Peek at it |

## Known limitations

- Some Chrome extensions use Chrome-only features and won't fully work. Extensions don't run in private tabs.
- Sites that need Widevine DRM, such as some streaming services, may not play video.
- No sync between Macs yet; use **Backup and restore** to move your data.
- Passkeys aren't supported yet.
- Mac only for now.

## Built with

- [Swift](https://www.swift.org), [SwiftUI](https://developer.apple.com/xcode/swiftui/) and [WebKit](https://webkit.org)
- [Readability](https://github.com/mozilla/readability) by Mozilla for reader mode (Apache License 2.0)
- [EasyList and EasyPrivacy](https://easylist.to) filter lists for Lume Shield

---

<div align="center">

Made by **MazeBeam Tech**

© 2026 MazeBeam Tech. All rights reserved.

</div>
