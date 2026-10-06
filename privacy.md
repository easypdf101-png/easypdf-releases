# Easy PDF — Privacy Policy

_Last updated: October 2026_

Easy PDF ("the app") is made by Dray, a sole proprietor in Toronto, Ontario, Canada. This policy explains what
happens to your information when you use Easy PDF on Android or Windows.

**The short version:** your documents stay on your devices. Easy PDF has no accounts, no ads, no analytics and no
tracking. When you sync or share, your files are encrypted on your device first, so nobody else — including us —
can read them.

## What stays on your device

- Your PDFs, notes, scans, books, highlights, signatures and settings are stored on your own phone or PC.
- Text recognition (OCR) and translation run on your device.
- The app keeps a small diagnostics log on your device to help fix problems. It never leaves your device unless
  you choose to share it with us (for example, by emailing it), and it is cleaned of file paths, email addresses
  and IP addresses first.

## Syncing your own devices and sharing with friends

When you link your phone and PC, or share a folder with a friend:

- On the same Wi-Fi, your devices talk to each other directly.
- Otherwise, files pass through our relay (a Cloudflare Worker with Cloudflare R2 storage). **Everything is
  end-to-end encrypted on your device before it is sent** (X25519 + XChaCha20-Poly1305). The relay only ever holds
  encrypted data and a hash of each access token — it does not have the keys and cannot read your files, their
  names or their contents.
- Encrypted copies are removed when they're no longer needed: pairing codes expire after a day, and a mailbox not
  used for 6 months is deleted.
- To let your other devices know something changed, the app registers a push notification token with Google's
  Firebase Cloud Messaging. This token identifies the app installation, not you, and is deleted from the relay when
  it stops working (for example, if you uninstall the app).

## Optional services you choose to use

- **Google Drive (optional):** if you sign in to Google Drive in Easy PDF, the app uses its own hidden app folder
  in your Drive (the `drive.appdata` permission). It cannot see your other Drive files. You can sign out at any
  time, which revokes the app's access.
- **Dictionary (optional):** when you look up a word, that word is sent to the free Dictionary API
  (dictionaryapi.dev) to get its definition. Nothing else is sent.
- **Microsoft Word (PC, optional):** "Edit in Word" and "Open in Word" open a copy in Word on your own PC.

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

You can delete any file in the app, unlink devices, stop sharing, sign out of Google Drive, or uninstall the app,
which removes its data from that device. To remove an encrypted mailbox from the relay right away, unlink all your
devices or contact us.

## Changes

If this policy changes, the new version will be posted at this address with a new date.

## Contact

Questions or requests: **easypdf101@gmail.com** 
