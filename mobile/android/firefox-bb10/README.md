# FoxBrowser BB10

A Firefox-inspired Android browser targeting BlackBerry 10 (Android API 18 - Jelly Bean runtime).

## Current Features
- Core WebView-based web rendering.
- Address bar with URL entry and basic "Go" logic.
- Navigation controls: Back, Forward, Refresh.
- Animated progress bar synced with WebView loading.
- Firefox-inspired UI (Navy and Orange theme).
- Holo-compatible styles for BB10 Android runtime.

## Planned Future Features (Second Steps)
As this is a foundation for a full browser, the following features are planned for future development:

### 1. Tab Management
- Support for multiple browser tabs.
- Tab switcher UI to view and manage open pages.
- "New Tab" button in the toolbar.

### 2. Bookmarks & History
- Ability to save and manage bookmarked pages.
- History view to revisit previously loaded URLs.
- SQLite integration for persistent storage of user data.

### 3. Settings & Configuration
- Custom user agent selection.
- Privacy settings (Clear cookies/cache).
- Default search engine configuration.

### 4. Integration with Mozilla Services
- Sync support for bookmarks and history via Firefox accounts.
- Integration with GeckoView (if performance on BB10 allows).

## Build Instructions
To build the project in this environment:
```bash
ANDROID_HOME=/home/jules/.mozbuild/android-sdk-linux ./gradlew :firefox-bb10:assembleDebug
```
The output APK will be located in `objdir/gradle/build/mobile/android/firefox-bb10/outputs/apk/debug/firefox-bb10-debug.apk`.
