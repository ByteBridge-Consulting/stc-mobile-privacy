# Intercity STC — Legal Pages

Public legal pages for the **Intercity STC** mobile app, hosted on GitHub Pages
so they can be linked from the Google Play Console and the App Store.

| Page | Live URL | Used for |
| --- | --- | --- |
| Privacy Policy | https://bytebridge-consulting.github.io/stc-mobile-privacy/ | Play Console *Privacy policy* field; App Store privacy URL |
| Delete Your Account | https://bytebridge-consulting.github.io/stc-mobile-privacy/account-deletion.html | Play Console **Data safety → Account deletion URL** |

Each page is a single self-contained HTML file — no build step, no dependencies.
Edit and push to `main`; Pages redeploys automatically.

## Who is who on these pages

The app is **operated by Intercity STC Coaches Ltd.**, who remain the data controller
under Ghana's Data Protection Act, 2012 (Act 843). The app is **developed and supported by
Byte Bridges Solutions**, who receive all account, privacy and support correspondence.

Both pages say this explicitly, so a user is not surprised to find the contact address on
a different domain from the operator's. Keep that framing if the pages are edited: dropping
the controller statement weakens the policy, and dropping the Byte Bridges line makes the
contact address look wrong.

## Why the deletion page exists

Google Play requires a **publicly reachable web URL** where users can request account
deletion, even though the app already offers in-app deletion on the Profile page. The URL
must work without signing in and without installing the app, so it has to be a plain static
page like this one.

The page documents both routes — in-app and by email — and states what is deleted versus
what is retained for tax and regulatory reasons. Play rejects deletion pages that promise
blanket deletion while the privacy policy describes retention, so the two pages must stay
consistent with each other.

## Still needs sign-off

The pages are complete and carry real contact details, but two claims are ours rather than
STC's, and should be confirmed before the Play submission:

- **Response times** — `account-deletion.html` section 2 commits to acknowledging within
  2 business days and completing verified deletions within 30 days. The 30 days matches
  Act 843; the 2 business days is an operational promise Byte Bridges has to be able to keep.
- **Retention period** — `account-deletion.html` section 3 and `index.html` section 5 say
  booking and payment records are kept "for the period required by Ghanaian tax, accounting,
  safety and transport regulations" without naming a number. If a reviewer asks for a
  specific period, agree one with STC and state it on both pages.

There is no phone number on either page. Email plus a postal address is a sufficient contact
route for Play and for Act 843; add a number to section 10 of the policy and section 5 of the
deletion page if you want one published.
