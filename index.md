# Fern — Privacy Policy

**Last updated: 2026-05-28**

## TL;DR

Fern doesn't collect, sell, share, or track anything about you. Everything you type into Fern stays on your device. We do not run analytics, we do not have ad SDKs, and we do not phone home.

The one exception is **optional device sync** — if you choose to pair two devices, Fern relays end-to-end encrypted blobs through a backend so your data can move between phones you own. The relay cannot read those blobs.

---

## What data Fern stores

When you use Fern, the following lives **locally on your device**, in the app's private storage:

- Transactions you log (amounts, dates, notes, tags, attached account/category)
- Accounts and wallets you set up
- Categories, budgets, recurring bills, savings goals, templates, receivables
- Your preferences (currency, theme, hide-balances toggle)
- A randomly-generated device ID (used only for sync identification)

This information **never leaves your device** unless you explicitly:
- Export it via Settings > Export CSV (you choose where to send the file)
- Back it up via Settings > Backup (you choose where to save the backup)
- Enable Sync (see below)
- Send feedback (you choose what to write and where to send it)

## Permissions Fern asks for

- **Local authentication (Face ID / Touch ID / device passcode)** — only if you opt into Device Lock in Settings. Used to gate access to the app. Authentication happens on your device only; Fern receives a yes/no result, not your biometric data.
- **Notifications** — for recurring bill reminders that you create yourself. Notifications are scheduled locally; nothing about them leaves your device.
- **Sharing / file access** — used only when you tap Export or Share. The OS share sheet is invoked; Fern does not read your other files.

## Optional sync

If you choose to pair two devices (Settings > Sync), the following happens:

- A symmetric encryption key is generated **on your device**.
- All your synced data is encrypted with that key **before** leaving your device.
- The encrypted blobs are stored on a Supabase backend.
- Your second device receives those blobs and decrypts them using the same key.
- **The Fern team cannot read your synced data.** The backend stores ciphertext only.
- Pairing is done via QR code or pairing string. Only devices you authorize can join your sync group.

You can leave your sync group at any time. Doing so revokes that device's access; existing data on the device stays.

## What Fern does NOT do

- We do not run analytics SDKs (no Firebase Analytics, no Mixpanel, no Amplitude, no Posthog).
- We do not run crash-reporting SDKs that send PII (Sentry would only be added with explicit user opt-in if at all).
- We do not run advertising SDKs.
- We do not have any social-login providers.
- We do not connect to your bank, your credit cards, or any financial institution.
- We do not share your data with any third party.
- We do not sell your data, ever, for any reason.

## Children's privacy

Fern is not directed at children under 13. We do not knowingly collect any data from children. Since Fern collects no data at all, this is incidentally satisfied.

## Changes to this policy

If we update this policy, the "Last updated" date at the top will change and the new version will be available at the same URL. Material changes will also be surfaced in an in-app notice on the next open after the change.

## Contact

If you have questions about this policy:

- Email: **edanuele@gmail.com**
- Or use Settings > Send feedback in the app, which routes to the same place.

---

*Fern is a privacy-first manual-entry budget tracker. No banks. No accounts. Just your money.*
