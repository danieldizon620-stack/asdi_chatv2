ASDI Chatroom Android v2.1 — Compact Chat Layout

CHANGES
- Removes the native floating PHOTO button at bottom right.
- Keeps camera/photo access through the existing chat attachment picker.
- Makes conversation bubbles compact and left/right aligned on phones.
- Places the message composer at the bottom with a compact header.
- Retains editable server URL, ASDI login, and existing notification logic.

ANDROID: Upload the project root to GitHub and run .github/workflows/build_apk.yml.
SERVER (optional but recommended): Back up group_chat_widget.php, then copy
server/group_chat_widget.php to asdi_ticketing/group_chat_widget.php and
server/assets/asdi_android_compact_v21.css to asdi_ticketing/assets/.
The server CSS makes the same layout work in a phone browser.
Note: no compiled APK is included. Native Android build and live chat testing pending.
