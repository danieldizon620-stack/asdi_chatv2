ASDI Chatroom Android v2.3 — Ticket Alerts + Logout + Mobile Layout

Features:
- Fixed server URL; no Server Settings.
- Chatroom opens directly after login (existing redirect rules).
- New-ticket alerts with available ticket fields and sound/vibration while app runs.
- Tap ticket notification to view full ticket in authenticated web page.
- Logout via Android app's top-right overflow menu.
- Responsive mobile chat bubbles and Bootstrap-style responsive CSS.
- No floating photo button.

SERVER INSTALL REQUIRED:
Copy BOTH server/mobile_ticket_notifications.php and server/mobile_logout.php to the asdi_ticketing root.
Existing config/app.php, users, tickets and customers tables are reused.
Ticket notifications are polled only while app is running, every 15 seconds.
On first run historical tickets are not notified.
The alert includes available ticket details; the ticket view contains full information.
Do not expose endpoint without require_login().
Server should be reachable from Android device.

ANDROID BUILD: Upload source project to GitHub and run .github/workflows/build_apk.yml.
This package is SOURCE ONLY, not a compiled or device-tested APK.
