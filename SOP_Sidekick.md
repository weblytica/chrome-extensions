Privacy Policy
--------------

**Last updated:** May 2, 2026

SOP Sidekick is a Chrome extension that displays a checklist in a side panel based on the URL of your active browser tab. This policy explains exactly what data the extension touches.

What the extension reads
------------------------

*   **The URL of your active tab.** Used only to compare against the URL patterns you’ve defined in your Google Sheet. The extension does not read the contents of any web page.
*   **A screenshot of your active tab.** Captured via Chrome’s `chrome.tabs.captureVisibleTab` API to display a small page preview in the side panel. The screenshot is held in memory only, never written to disk, and never transmitted off your computer.
*   **Your Google Sheet, when configured.** Fetched via the public CSV export endpoint. The Sheet must be shared as “Anyone with the link — Viewer.” We never receive a copy; the request goes directly from your Chrome to Google.

What the extension stores
-------------------------

*   **Settings** — Sheet URL/ID, Sheet tab GID, webhook URL, webhook key, and theme preference. Stored in `chrome.storage.sync`, which Chrome syncs across your signed-in Chrome installs. Nothing is sent to us.
*   **Checklist progress** — which items you have checked off. Stored in `chrome.storage.session`, which Chrome clears when the browser closes.
*   **A short cache of your Sheet contents** — stored in `chrome.storage.local` for up to 5 minutes to avoid re-fetching on every navigation.

What the extension transmits
----------------------------

The extension makes only two kinds of outbound network requests:

1.  **A request to Google Sheets** (`docs.google.com`) to fetch your configured Sheet. Triggered when you set up the Sheet, click Refresh in the side panel, or after the cache expires.
2.  **A POST to your webhook URL**, only if you have configured one and only when you click **Log completion**. The body contains: timestamp, the active tab’s URL and title, the SOP’s title and pattern and source-doc link, the full list of checklist items with their completed/not-completed status, and (if you set one) the webhook key. You — not we — control where this data goes.

What the extension does NOT do
------------------------------

*   It does not read the contents of any web page you visit.
*   It does not modify any web page you visit.
*   It does not send any analytics, telemetry, error logs, or diagnostic information to us or to any third party.
*   It does not require an account, login, or any personal information.
*   It does not use cookies.
*   It does not advertise.
*   It does not sell, trade, or transfer any user data.

Permissions and why we ask for them
-----------------------------------

Permission

Why

`sidePanel`

The extension’s main UI is a side panel.

`storage`

Save your settings and checklist progress in Chrome’s local storage.

`tabs`

Read the active tab’s URL to compare against your patterns; update the badge on the toolbar icon per tab.

`activeTab`

Capture a screenshot of the active tab for the in-panel preview.

`https://docs.google.com/*`, `https://script.google.com/*`

Fetch your Sheet via the public CSV export.

Optional `https://*/*`, `http://*/*`

Requested only when you save a webhook URL, so the extension can POST completion data to that host.

Children
--------

The extension is not directed at children under 13.

Changes to this policy
----------------------

If we change anything material, we will update the date at the top of this page and (if you have the extension installed) the side panel’s footer link will continue to point here so you can re-read it.

Contact
-------

Questions or concerns: **andy@weblytica.com**

For an open-source view of exactly what the extension does, the code is available at the project’s GitHub repository.
