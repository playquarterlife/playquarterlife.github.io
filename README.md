# Quarterlife waitlist site

A plain static site (no build step): `index.html`, `thanks.html`, `img/`, `fonts/`. Hosted on GitHub Pages.

## Setup: two things to paste
Both are at the top of the `<script>` near the bottom of `index.html` (and the Discord one in `thanks.html` too):
- `KIT_FORM_ACTION`: Kit → Grow → Landing Pages & Forms → your form → Embed → HTML. Copy the link inside `action="…"` (looks like `https://app.kit.com/forms/1234567/subscriptions`).
- `DISCORD_INVITE`: Discord → server name → Invite People → Edit invite link → Expire after **Never** → copy.

Until they're filled in, the form shows "Sign-ups aren't switched on yet" and the Discord buttons stay hidden.

## Kit settings for the form
- Form settings → **Incentive / confirmation email**: on (double opt-in, so only real addresses join).
- Form settings → **After subscribing**: redirect to `https://<your site>/thanks.html`.
- The beta tick box sends a custom field named **beta** (value `yes`). Create a custom field called `beta` in Kit so it's saved (if Kit's free plan doesn't allow custom fields, switch the box to a tag or a second form). Then filter subscribers by `beta = yes` to find testers.

## Privacy
No analytics or trackers on this site. The only data collected is the email (and the beta tick), stored in Kit.

## Rights
© 2026 Quarterlife. All rights reserved. The art, screenshots, text and design on this site belong to Quarterlife and may not be reused without permission (see `NOTICE`).

The font Tiny5 is under the SIL Open Font License, included as `fonts/Tiny5-OFL.txt`.
