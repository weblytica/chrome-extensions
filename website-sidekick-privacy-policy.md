# Website Sidekick Privacy Policy

**Last Updated: August 2026**

This policy covers the Website Sidekick Chrome extension.

The short version: the extension has no server. Weblytica never receives your data.
Everything it stores stays in your own browser, and everything it sends goes to your
own accounts.

## Who We Are

Weblytica, LLC publishes the Website Sidekick extension. If you have a question about
this policy or your data, email <andy@weblytica.com>.

## What The Extension Stores

Everything below is saved in your browser's local extension storage, on your own
computer. None of it is sent to Weblytica. There is no Weblytica account, server, or
database behind the extension.

| What | Why it is stored |
|------|------------------|
| **Site settings** | For each website you choose to edit: the config folder address, the GitHub repository name, the branch, and the folder path inside that repository. |
| **Your GitHub personal access token** | You create this in your own GitHub account and paste it in. It is what lets your edits be committed to your repository. |
| **Your ImageKit key** (optional) | Only stored if you choose to route uploaded images through your own ImageKit account. |
| **Unsaved drafts** | While you have edits you have not published yet, a copy is kept so you do not lose them by switching tabs or closing the browser. Drafts are deleted as soon as you publish or discard them. |

## Where Your Information Goes

The extension talks to three kinds of destination, all of them yours, and only when
you act:

- **The website you are editing.** The extension reads the public content files that
  site publishes, so it knows what is editable on the page you are on.
- **GitHub.** When you press Save, your edited content and your token are sent to
  GitHub's API to create a commit in the repository you configured. This is a direct
  connection between your browser and GitHub.
- **ImageKit.** Only if you have entered an ImageKit key. Images you upload are sent
  to your ImageKit account to be optimized before they are committed.

There are no other network destinations. The extension contains no analytics, no
tracking, no advertising, and no error reporting service.

## What We Do Not Do

We do not collect, receive, see, sell, rent, or transfer your data to anyone. We do
not use it to build profiles, target advertising, or train models.

Your tokens are never transmitted anywhere except to GitHub and ImageKit, which are
the services those credentials belong to.

The extension's use of information is limited to providing the editing feature you
installed it for, which is the single purpose described on its Chrome Web Store
listing.

## Which Sites It Can Access

The extension does not request access to the web at large when you install it. It asks
for permission one website at a time, and only for a site you have explicitly set up
for editing. Sites you never grant are never read, and removing a site from the
extension's settings hands that permission back.

## How To Remove Your Data

1. Open the extension's settings and use the remove control next to any saved site.
   That erases its settings and its token.
2. Removing the extension from Chrome deletes everything it stored, immediately and
   permanently.
3. Revoke the personal access token in your GitHub account settings. That token exists
   independently of the extension, so removing the extension does not revoke it.

## Children

The extension is a professional tool for people who maintain websites. It is not
directed at children and we do not knowingly collect information from anyone under 13.

## Changes To This Policy

If the extension ever changes what it stores or where it sends it, this page is updated
and the date at the top changes with it.

## Contact

Questions about this policy or the extension? Email <andy@weblytica.com> and a real
human will get back to you.

---

*This policy is a plain-language starting point, not legal advice. If you operate in a
regulated market, have it reviewed by a professional to be sure it fits your
obligations.*
