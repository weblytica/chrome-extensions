# REACH UP Networking — Privacy Policy

**Effective date:** October 28, 2026
**Publisher:** Weblytica, LLC

> **The short version:** your contacts and notes stay on your device. We
> (Weblytica) never see, collect, or receive any of your data. Information
> only leaves your computer when *you* turn on Google Drive backup or *you*
> click Send to a webhook you configured. There are no analytics, no ads,
> and nothing is ever sold.

## What REACH UP does

REACH UP Networking is a Chrome extension that turns meeting chat transcripts
you paste into a searchable contact list with notes, kept in Chrome's side
panel. All processing happens locally in your browser.

## Information the extension stores

When you paste a chat transcript, the extension extracts contact details
(names, email addresses, phone numbers, LinkedIn URLs, websites) and stores
them — together with any notes you write, your webhook configurations, and
your settings — in Chrome's local extension storage (`chrome.storage.local`)
on your device only.

- No data is transmitted to Weblytica. We operate no servers for this extension.
- No analytics, telemetry, crash reporting, or tracking of any kind.
- No data is sold, rented, or shared with third parties by us — ever.

## When data leaves your device

Exactly three actions send data anywhere, and you initiate each one:

| Action | What is sent | Where it goes |
| --- | --- | --- |
| Google Drive backup (opt-in) | Your contacts and notes | A Google Sheet in *your own* Google Drive account |
| Webhook send (per click) | One contact and its notes, as JSON | The URL you configured (e.g. your CRM or automation platform) |
| CSV export | Your contact list | A file downloaded to your computer |

## Google account access

If you enable Google Drive backup, the extension asks Google for two narrow
permissions:

- **Create and edit files it creates** (`drive.file` scope) — this lets the
  extension create one backup spreadsheet and update it. It cannot see, open,
  or modify any other file in your Drive.
- **Your email address** (`userinfo.email` scope) — shown in the panel header
  so you can confirm which account the backup goes to.

REACH UP's use of information received from Google APIs adheres to the
[Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy),
including its Limited Use requirements. Google data is used only to provide
the backup feature you enabled; it is never transferred to anyone else, never
used for advertising, and never read by humans.

You can disconnect at any time with **Disconnect & Sign Out** in the
extension's Storage Options, which revokes the extension's access with
Google. You can also revoke access from your
[Google Account permissions page](https://myaccount.google.com/permissions).

## Webhooks

Webhook destinations are entirely your choice. The extension sends data to a
webhook only when you click Send on a contact, and only to URLs you added
yourself. The optional shared secret you configure is stored locally and sent
as a request header so your endpoint can verify the sender. Webhook URLs and
secrets are never included in Google Drive backups. The privacy practices of
the receiving service are governed by that service's own policy.

## Deleting your data

- **In the extension:** Storage Options → Delete All Data permanently erases
  all contacts, notes, and settings from your device.
- **Uninstalling the extension** also removes its local storage.
- **Google Sheet:** the backup spreadsheet lives in your Drive and remains
  yours; delete it from Drive whenever you like.

## Children

REACH UP is a professional networking tool and is not directed at children
under 13. We do not knowingly collect information from children.

## Changes to this policy

If this policy changes, the updated version will be posted at this URL with a
new effective date, and material changes will be noted in the extension's
Chrome Web Store listing changelog.

## Contact

Weblytica, LLC
Email: [andy@weblytica.com](mailto:andy@weblytica.com)
Web: [weblytica.com](https://weblytica.com)
