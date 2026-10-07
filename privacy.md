# Easy PDF — Privacy Policy

_Last updated: October 2026 (version 3.4)_

Easy PDF ("the app") is made by Dray, a sole proprietor in Toronto, Ontario, Canada. This policy explains what
happens to your information when you use Easy PDF on Android or Windows.

**The short version:** your documents stay on your devices. Easy PDF has no accounts, no ads, no analytics and no
tracking. When you sync or share, your files are encrypted on your device first, so nobody else — including us —
can read them.

## What stays on your device

- Your PDFs, notes, scans, highlights, signatures and settings are stored on your own phone or PC. (On the
  Microsoft Store version for Windows, your library is kept in your Documents folder, in "Easy PDF", so
  uninstalling the app never deletes your files.)
- Translating a page runs on your device.
- The app keeps a small diagnostics log on your device to help fix problems. It never leaves your device unless
  you choose to share it with us (for example, by emailing it), and it is cleaned of file paths, email addresses
  and IP addresses first.

## Syncing your own devices and sharing with friends

When you link your phone and PC, or share a folder with a friend:

- On the same Wi-Fi, your devices talk to each other directly. (You can turn this off with "Relay only".)
- Otherwise, files up to 25 MB each pass through our relay; bigger files wait until your devices are on the same
  Wi-Fi. The relay is a Cloudflare Worker with Cloudflare R2 storage. **Everything is
  end-to-end encrypted on your device before it is sent** (X25519 + XChaCha20-Poly1305). The relay only ever holds
  encrypted data and a hash of each access token — it does not have the keys and cannot read your files, their
  names or their contents.
- Encrypted copies are removed when they're no longer needed: pairing codes expire after a day, and a mailbox not
  used for 6 months is deleted.
- To let your other devices know something changed, the app registers a push notification token with Google's
  Firebase Cloud Messaging. This token identifies the app installation, not you, and is deleted from the relay when
  it stops working (for example, if you uninstall the app).

## Optional services you choose to use

- **OneDrive and Google Drive folders on your PC/phone (optional):** opening or saving files there uses your
  computer's or phone's own file system; Easy PDF doesn't connect to those services itself.
- **Email and other apps (optional):** when you share a file, your device's own share options send it; Easy PDF
  doesn't see where it goes.

## What we don't do

- We don't sell, rent or share your information.
- We don't show ads or use advertising IDs.
- We don't use analytics or crash-reporting services.
- We don't require an account, email address or phone number.

## Permissions

- **Camera** — to scan documents and take photos for notes (only when you use those features).
- **Notifications** — to tell you when a sync or shared file arrives.
- **Files / storage** — only the files and folders you choose (for example, "Save a copy to phone").
- **Fingerprint / face unlock** — for the optional app lock. Android checks it; Easy PDF never sees your fingerprint or face.

## Children

Easy PDF is not directed at children under 13 and does not knowingly collect information from children.

## Your choices

You can delete any file in the app, unlink devices, stop sharing, or uninstall the app, which removes its settings
from that device (on Windows, your library folder stays until you delete it). To remove an encrypted mailbox from the relay right away, unlink all your
devices or contact us.

## Changes

If this policy changes, the new version will be posted at this address with a new date.

## Contact

Questions or requests: **easypdf101@gmail.com**
