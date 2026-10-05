# Retatrutide Community Poll (public voting page)

Live: https://discoveranytime.github.io/retatrutide-poll/

Fast, mobile-friendly, single-file poll page. Themed from the poll's `theme`
JSON (Retatrutide palette by default). No trackers, no personal info required.

Part of the reusable community poll system — full docs, backend (Supabase),
and admin dashboard in the `poll-admin` repo. See its README for setup.

## Configure
Edit `config.js`:
```js
window.POLL_CONFIG = {
  SUPABASE_URL: "https://YOUR_PROJECT_REF.supabase.co",
  SUPABASE_ANON_KEY: "YOUR_ANON_KEY",
  TURNSTILE_SITEKEY: ""   // optional CAPTCHA
};
```
Empty `SUPABASE_URL` = preview mode (local votes only, badged).

## Other polls
`?poll={slug}` loads any poll, e.g. `?poll=tirzepatide-interests`.
