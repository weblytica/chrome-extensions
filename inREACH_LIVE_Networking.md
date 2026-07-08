# inREACH LIVE Networking

Effective date: 4/21/2026

Publisher: Weblytica, LLC Contact for privacy questions: chome-store@weblytica.com

This policy explains what data the inREACH LIVE Networking Chrome extension (“the extension”) handles, where it goes, and what you can do about it. We wrote it in plain language — no dark patterns, no buried caveats.

Summary
We operate no servers. Your data stays on your device by default.
No analytics, no tracking, no telemetry. The extension does not phone home, ever.
Optional Google Drive backup goes only to your own Drive — we have no access to it.
Optional webhook sends go directly from your browser to the URL you configured — we don’t see, log, or relay the request.
You can delete everything at any time from the Storage Options → Delete All Data button.
What data the extension handles
1. Contact information you choose to import
When you paste a Zoom chat transcript and click “Clean Chat History,” the extension extracts these fields from the transcript locally, in your browser:

Name
Email address
Phone number
LinkedIn profile URL
Personal website URL
Date (extracted from the transcript)
This is information other people shared in a chat that you had access to, pasted by you into the extension.

2. Notes you write
You can add free-text notes to any contact. Each note is timestamped with the date and time you saved it. Notes can be edited or deleted at any time.

3. Webhook configurations
If you choose to configure one or more webhook destinations (for example to send contacts to Make, Zapier, or a CRM), the extension stores:

The name you give each webhook
The URL you provided
Any optional shared secret you entered for that webhook
These are saved locally on your device only. They are never transmitted to us, synced through Chrome Sync, or mirrored to Google Drive.

4. Google authentication token (only if you enable Drive backup)
If — and only if — you explicitly enable the optional Google Drive backup feature, Chrome’s built-in identity system stores an OAuth 2.0 token that authorizes the extension to access the single Google Sheet it creates in your Drive. This token lives in Chrome’s token cache and is managed by Chrome; we never receive it.

The OAuth scopes requested are:

https://www.googleapis.com/auth/drive.file — limited to files the extension creates. The extension cannot see, list, read, or modify any other file in your Drive.
https://www.googleapis.com/auth/userinfo.email — used to display your email address in the extension’s header so you can verify which Google account you are signed in with. The email is never stored, transmitted to us, or used for any other purpose.
You can disconnect and revoke the extension’s Google access at any time via the “Disconnect & Sign Out” button in the extension, or at https://myaccount.google.com/permissions.

Where your data is stored
By default: only on your device.

The extension uses Chrome’s built-in chrome.storage.local API to store contacts, notes, and webhook configurations. This storage lives in your local Chrome profile and is never synced through Chrome Sync, never uploaded to our servers (we operate none), and never transmitted to any third party.

Optional: in your own Google Drive.

If you enable the optional Google Drive backup, the extension creates a single spreadsheet named “inREACH LIVE Networking” in your Drive and mirrors your contacts and notes into it. This spreadsheet lives entirely under your control in your own Google account.

You can:

Open the sheet at any time from the extension
Edit the sheet directly in Google Sheets (your local data will be overwritten by the next sync)
Delete the sheet from your Drive whenever you want
Disconnect the extension from Drive without deleting the sheet
Webhook URLs are never synced to Drive. Because they may contain secrets, they remain local-only.

Third-party services
The extension communicates with the following third parties:

Google APIs (only if you enable Drive backup)
Google Drive API — to create and update the backup spreadsheet
Google Sheets API — to read/write the contents of the spreadsheet
Google OAuth 2.0 service — to authenticate you with your Google account
Google userinfo endpoint — to retrieve your email address for display in the extension header
Google’s handling of your interaction with these APIs is governed by Google’s own Privacy Policy: https://policies.google.com/privacy

Webhook endpoints (only if and when you explicitly send)
When you configure a webhook URL and manually click “Send” on a contact, the extension makes a direct HTTPS POST request from your browser to the URL you provided. The request contains the contact’s data and notes as JSON.

We have no involvement in, visibility into, or logging of these requests. The privacy policy of the destination service (Make, Zapier, your CRM, etc.) governs what happens to the data you send there.

What the extension does NOT do
Does not transmit any data to the publisher (Weblytica, LLC). We operate no servers and no database.
Does not track your browsing activity or the sites you visit.
Does not inject content scripts into web pages.
Does not use cookies, web beacons, fingerprinting, or analytics of any kind.
Does not share your data with third parties except as you direct (Drive backup, webhook sends).
Does not use your data for advertising or to determine creditworthiness.
Does not sell your data to anyone.
Does not use remote code. All JavaScript executed by the extension is bundled within the extension package and reviewed at submission.
Deleting your data
You can delete all locally stored data at any time:

Open the extension side panel
Click the storage indicator in the footer (“Using Local Storage” or “Using Google Drive Storage”)
Click “Delete All Data”
Confirm the deletion
This immediately removes all contacts, notes, and webhook configurations from your device.

Google Drive backup sheet (if any) must be deleted separately from your Google Drive. The extension does not delete files in your Drive as part of “Delete All Data” so you retain full control of your backup even after uninstalling the extension.

To revoke the extension’s Google Drive access without deleting any data, use the “Disconnect & Sign Out” button in the extension, or visit https://myaccount.google.com/permissions.

Your rights
Because your data never leaves your device (unless you opt into backup, in which case it goes only to your own Google account), we cannot access, delete, correct, or export your data on your behalf — you have complete and direct control from within the extension and your own Google account.

Children’s privacy
The extension is not directed at children under 13. It handles only contact information that users themselves paste into it from their own professional networking events.

Changes to this policy
If we materially change how the extension handles data, we will:

Update this page with a new “Effective date”
Note the change in the extension’s release notes on the Chrome Web Store
For significant changes (e.g., new data categories, new third-party integrations), show an in-extension notice on first launch after the change
Contact
Questions, concerns, or requests about privacy can be sent to: chome-store@weblytica.com

We read every message and respond personally.
