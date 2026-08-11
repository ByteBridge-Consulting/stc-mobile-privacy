# Intercity STC — Privacy Policy

Public legal pages for the **Intercity STC** mobile app, hosted on GitHub Pages
so they can be linked from the Google Play Console and the App Store.

| Page | Live URL | Used for |
| --- | --- | --- |
| Privacy Policy | https://bytebridge-consulting.github.io/stc-mobile-privacy/ | Play Console *Privacy policy* field; App Store privacy URL |
| Delete Your Account | https://bytebridge-consulting.github.io/stc-mobile-privacy/account-deletion.html | Play Console **Data safety → Account deletion URL** |

Each page is a single self-contained HTML file — no build step, no dependencies.
Edit and push to `main`; Pages redeploys automatically.

## Why the deletion page exists

Google Play requires a **publicly reachable web URL** where users can request account
deletion, even when the app already offers in-app deletion (which this app does, on the
Profile page). The URL must work without signing in and without installing the app, so it
has to be a plain static page like this one.

The page documents both routes — in-app and by email — and states what is deleted versus
what is retained for tax and regulatory reasons. Play rejects deletion pages that promise
blanket deletion while the privacy policy describes retention, so the two pages must stay
consistent with each other.

## Before this is submitted to Play

Both pages contain **placeholders** that must be replaced with STC's real details:

- `index.html` section 10 — privacy contact email, postal address, phone number.
- `account-deletion.html` sections 2 and 5 — support email address.

Also confirm with STC operations before publishing:

- the response and completion times quoted in `account-deletion.html` section 2, and
- the retention period for booking and payment records in section 3.

Google Play checks that the contact route on these pages actually works.
