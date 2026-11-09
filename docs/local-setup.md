# Local lab setup

This project was demonstrated with GoPhish and Mailpit running locally. The tools themselves are third-party software and are intentionally not bundled in this repository. Obtain them from their official project releases and review their licenses.

## Demonstrated local endpoints
- GoPhish admin interface: `https://127.0.0.1:3333`
- GoPhish phishing server: `http://127.0.0.1:8080`
- Mailpit web interface: `http://127.0.0.1:8025`
- Mailpit SMTP: `127.0.0.1:1025`

These are local-only demonstration settings, not public deployment settings. Keep the admin interface bound to localhost. Do not publish GoPhish databases, recipient lists, campaign exports, credentials, private keys, or real email addresses. Configure your own test recipient and SMTP settings.

## Campaign workflow
1. Start Mailpit and verify its local web inbox.
2. Start GoPhish and sign in to its local admin interface.
3. Configure a sending profile to use Mailpit SMTP at `127.0.0.1:1025`.
4. Create a test email template using the `{{.FirstName}}` and `{{.URL}}` placeholders.
5. Create a landing page containing awareness guidance. Keep credential/data capture disabled.
6. Create a group containing only an address you control, then run a local campaign.
7. Review delivery, open, and click events in the campaign results.
8. Confirm that no submitted credentials or sensitive data were collected.

## Safety and scope
This repository documents a controlled awareness exercise conducted with a local test recipient and a local mail-capture service. Run simulations only with explicit authorization and informed scope. Never target third parties or collect passwords.
