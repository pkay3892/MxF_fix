# The Gap

A private habit tool for one person. Everything is stored in your phone's
browser storage — no account, no server, nothing leaves the device.

## Put it on your Android phone

1. Create a new GitHub repository (public is fine — nothing personal is in the code).
2. Upload all five files to the root of the repo:
   index.html, manifest.webmanifest, sw.js, icon-192.png, icon-512.png, icon-maskable.png
3. Repo → Settings → Pages → Source: "Deploy from a branch" → Branch: main, folder: / (root) → Save.
4. Wait a minute, then open the URL GitHub gives you (https://<user>.github.io/<repo>/) in Chrome on your phone.
5. Chrome menu (⋮) → "Add to Home screen" → Install.

It now opens full-screen with its own icon and works offline.

## Reminders

The app deliberately does not nag you. Set these as repeating reminders on the
phone instead, with the text in the reminder itself so you never have to open anything:

- 08:30 daily — "Turn toward. Look up when she says something small."
- 21:30 daily — "20-second log."
- Sunday 11:00 — "Weekly check-in with F. 20 minutes."
- Before each protected time block — "Phone away."

## Updating it

Edit index.html in GitHub, commit, and bump `var CACHE = "gap-v1"` in sw.js to
"gap-v2" so the phone picks up the new version instead of the cached one.
