<div align="center">

# Lume

**Browse the future.**

A calm, minimal browser for Mac, written in Swift and powered by WebKit, with vertical tabs, separate spaces and one command bar.

[Download](../../releases) · [Features](#features) · [Shortcuts](#keyboard-shortcuts)

</div>

---

> **Lume is in alpha.** Expect rough edges, changing features and the occasional bug. Feedback is welcome: open an issue and tell us what you ran into.

## About

Lume is a native macOS web browser written in **Swift** with **SwiftUI**. It renders pages with **WebKit**, the same engine that powers Safari, so most sites work as you'd expect while the app stays light and feels at home on a Mac.

## Features

- **Vertical tabs:** your tabs live in a sidebar, where titles stay readable even with a lot open.
- **Spaces:** keep work, school and home apart. Each space has its own tabs, color and separate logins.
- **Command bar:** search, open a site or jump to any open tab from one place.
- **Pinned tabs:** pin the sites you live in to a tidy grid at the top of the sidebar.
- **Compact mode:** hide the sidebar so the page fills the window, and hover the left edge to bring it back.
- **Private tabs:** open an incognito tab that leaves nothing behind.
- **History:** look back at where you've been, and clear it whenever you like.
- **Light and dark:** follows your Mac, or pick a side in Settings.

## Requirements

| | |
|---|---|
| **Operating system** | macOS 14 (Sonoma) or later |

## Install

1. Download the latest `Lume.dmg` from [Releases](../../releases).
2. Unzip it and drag **Lume.app** into your **Applications** folder.
3. Open it.

### "Lume can't be opened"

Alpha builds aren't notarized with Apple yet, so macOS Gatekeeper may block the first launch. To open it anyway, do either of these:

- Right-click **Lume.app**, choose **Open**, then choose **Open** again.
- Or run this in Terminal:

  ```bash
  xattr -cr /Applications/Lume.app
  ```

## Keyboard shortcuts

| Shortcut | Action |
|---|---|
| ⌘T | New tab |
| ⌘L | Open location |
| ⌘W | Close tab |
| ⌘N | New window |
| ⇧⌘N | New incognito tab |
| ⌘R | Reload |
| ⌘[ and ⌘] | Back and forward |
| ⌘S | Show or hide the sidebar |
| ⌘Y | Show history |
| ⌥⇧⌘S | Save page as… |

## Known limitations

- Lume is built on WebKit, so Chrome extensions aren't supported.
- Sites that need Widevine DRM, such as some streaming services, may not play video.
- Mac only for now.

## Built with

- [Swift](https://www.swift.org)
- [SwiftUI](https://developer.apple.com/xcode/swiftui/)
- [WebKit](https://webkit.org)

---

<div align="center">

Made by **MazeBeam Tech**

© 2026 MazeBeam Tech. All rights reserved.

</div>
