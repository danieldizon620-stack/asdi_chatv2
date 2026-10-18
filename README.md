# ASDI Chatroom Android v2.0

Android WebView source for **chatroom-only** ASDI Ticketing access.

## Features
- Starts on editable **Server Settings** screen, no automatic connection.
- Save & Connect opens `chat_window.php` at your chosen ASDI Ticketing base URL.
- Server Settings button remains accessible while connected.
- Uses existing server login; redirects standard `index.php` / `dashboard.php` landing pages to chatroom.
- Camera/photo/file picker from previous version.
- Red in-app new-message counter and Android notification sound while app is running and the WebView can poll.

**Limits:** New-message detection uses increasing message IDs, not a per-user read receipt; it can count your own messages and may miss messages beyond the server's 50-message response. Android may suspend polling while backgrounded; this is **not reliable push notification**. Launcher-icon dots are controlled by Android launchers and may not appear. The uploaded Windows installer is unrelated to the Android build and cannot be converted into an APK.

## Build via GitHub Actions
1. Upload **contents of this `android` directory** to the repository root (so `settings.gradle` is at root).
2. GitHub Actions → **Build ASDI Chatroom APK** → Run workflow.
3. Download the artifact **ASDI-Chatroom-Server-Settings-APK**.
4. Install `app-debug.apk` on an Android phone (allow installation from your chosen source).

Requires reachable server from the phone, existing ASDI login, and HTTPS for production use. The included default `http://100.69.232.118:8080/asdi_ticketing/` is only a starting value.

This package is source code. It has not been compiled into an APK in this environment.
