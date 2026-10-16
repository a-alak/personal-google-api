# Ali’s Personal Google API Client

A small static information site for a personal Google OAuth client used with rclone and ad hoc API tools. Plain HTML and CSS; no build step, dependencies, JavaScript, or external fonts.

## Google OAuth consent screen URLs

- Application name: **Ali’s Personal Google API Client**
- Home page: https://a-alak.github.io/personal-google-api/
- Privacy policy: https://a-alak.github.io/personal-google-api/privacy.html
- Terms of service: https://a-alak.github.io/personal-google-api/terms.html

## Preview locally

```sh
python3 -m http.server 8000
```

Open http://localhost:8000. The site supports narrow screens and the system light/dark preference.

## Publishing

GitHub Pages serves the root of the `main` branch. Push changes to that branch to publish them. `.nojekyll` keeps the site as plain static files.

## Maintaining the policies

Keep the app name, account access, storage practices, and policies consistent with the actual client. Update the effective dates when changing the policies. Public repository issues are the contact channel; never post private account information there.

This repository must never contain OAuth secrets, tokens, rclone configuration, or Google account data.

## Google setup notes

Publishing this site does not publish or verify the OAuth client in Google Cloud. Configure the consent screen and publishing status separately. Personal-only use may qualify for Google's personal-use verification exception; an unverified-app warning and user cap may still apply. External apps left in Testing typically receive refresh tokens that expire after seven days when requesting scopes beyond basic identity.

If Google requires domain-ownership verification for your application, use a domain you own and can verify in Google Search Console. You cannot verify ownership of the shared `github.io` domain. A custom domain can still be hosted on GitHub Pages; update all consent-screen and README URLs if you switch.
