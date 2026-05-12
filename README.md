# Akoo Threads OAuth Test Page

This repository hosts the public HTTPS callback page for the Akoo Threads OAuth setup.

## URLs

- Test page: `https://tslj0427.github.io/akoo-threads-oauth/`
- OAuth Redirect URI: `https://tslj0427.github.io/akoo-threads-oauth/auth/callback/`

## Security Boundary

This static page does not store or request the Threads App Secret.

It can:

- Build the Threads OAuth authorization URL.
- Redirect the user to Meta / Threads authorization.
- Receive the authorization `code` in the callback URL.

It cannot safely exchange the authorization code for an access token, because token exchange requires the App Secret and must be done server-side or in a local secure environment.
