# UA Cinema Install

Static GitHub Pages site for installing UA Cinema and opening shared links.

Published site:

```text
https://koss-shtukert.github.io/ua-cinema-install/
```

Latest Android release:

```text
https://github.com/koss-shtukert/rd_flutter_project/releases/latest
```

Live update manifest:

```text
https://pub-b9c840137f154243adcb0088e4afba66.r2.dev/updates.json
```

## What Is UA Cinema

UA Cinema is a Flutter app for Ukrainian movies, series, anime, cartoons, and
Android TV playback. It merges multiple content sources into one catalog,
supports HLS playback, Chromecast, profiles, favorites, and continue watching.

## Install

Open the install page:

```text
https://koss-shtukert.github.io/ua-cinema-install/
```

The page reads the latest Android APK URL from `updates.json`. If that request
is unavailable in the browser, it falls back to the latest GitHub Release.

## Shared Links

Shared UA Cinema links use HTTPS first:

```text
https://koss-shtukert.github.io/ua-cinema-install/s/?id=<share-id>
```

The page then tries to open the app:

```text
uacinema://share/<share-id>
```

Pretty links also work through `404.html` fallback:

```text
https://koss-shtukert.github.io/ua-cinema-install/s/<share-id>
```

## GitHub Pages Setup

In this repository:

1. Open `Settings`.
2. Open `Pages`.
3. Set `Source` to `Deploy from a branch`.
4. Select branch `main`.
5. Select folder `/root`.
6. Save.

GitHub Pages will publish `index.html` from the repository root.
