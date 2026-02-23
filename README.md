# CricketLive Releases

Release artifacts and auto-update feed for [CricketLive](https://github.com/ashbridgewater/CricketLive).

## Download

Download the latest version from the [Releases page](https://github.com/ashbridgewater/CricketLive-releases/releases/latest).

### Installation

1. Download **CricketLive.dmg**
2. Open the DMG and drag CricketLive to your Applications folder
3. On first launch: right-click the app → **Open** (required once since the app is not notarized)
4. CricketLive appears as a cricket ball icon in your menu bar

### Updates

CricketLive checks for updates automatically via [Sparkle](https://github.com/sparkle-project/Sparkle). When a new version is available, you'll be prompted to install it. You can also check manually in Settings → Updates.

## What's in this repo

| File | Purpose |
|------|---------|
| `appcast.xml` | Sparkle update feed — the app polls this file to check for new versions |
| Releases | Each release contains a `.dmg` (for users) and `.zip` (for Sparkle auto-updates) |

## Why a separate repo?

The source code lives in a private repo. Sparkle needs to poll `appcast.xml` and download updates without authentication, so release artifacts are hosted here in a public repo. The app's `SUFeedURL` points to:

```
https://raw.githubusercontent.com/ashbridgewater/CricketLive-releases/main/appcast.xml
```

## Requirements

- macOS 13.0 (Ventura) or later
