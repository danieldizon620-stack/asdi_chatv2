ASDI Chatroom Android v2.2 — No Server Settings

The application now opens the fixed ASDI chatroom URL immediately:
http://100.69.232.118:8080/asdi_ticketing/chat_window.php

If the user is not logged in, the server's existing login page appears.
After login, the WebView redirects common dashboard URLs to chat_window.php.

- Removed the Server Settings screen and Server button.
- Retained compact mobile chat layout and no floating PHOTO button.
- Retained camera/photo attachments via the chat composer.
- Retained existing notification and red in-app unread badge logic.
- Retained the optional server-side mobile CSS/widget override.

To change the server later, edit DEFAULT_BASE in
app/src/main/java/com/asdi/chatroom/MainActivity.java and rebuild.

Upload project to GitHub and run .github/workflows/build_apk.yml.
This ZIP contains source code, not a compiled APK.
