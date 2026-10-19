ASDI Chatroom v2.4 — Unified (+) Composer Menu

The chat composer now has one (+) button for:
- Attach file or photo
- Take photo
- Emojis (including animated emojis)
- Remove attached file (only visible when relevant)
- Cancel replacement (only visible when relevant)

The original message-sending, attachment, emoji, replacement, deletion and notification logic is retained.
The floating PHOTO button remains removed.

INSTALL SERVER:
Back up the existing group_chat_widget.php and copy
server/group_chat_widget.php to your asdi_ticketing directory.
This is REQUIRED because the APK displays the server-hosted PHP chat interface.

ANDROID:
This ZIP also includes the Android v2.3 source project unchanged.
Upload project root to GitHub and run the build workflow if you want to rebuild the APK.
If only the PHP widget is updated, existing installed APKs can display the new composer
after refreshing the chat page, without reinstalling the APK.

The user-provided ZIP contained only app-debug.apk (a compiled APK), not editable source.
The included Android source comes from the previously developed v2.3 project.
This is source, not a compiled or tested APK.
