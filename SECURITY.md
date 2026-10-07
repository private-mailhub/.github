# Security

## Reporting a vulnerability

Please do not open a public issue for a security vulnerability. Report it privately by emailing
[contact@private-mail.com](mailto:contact@private-mail.com).

## Security guidance

- Primary email addresses and reply-routing values are encrypted with AES-256-GCM before they are
  stored in the database or cache.
- `VITE_ENCRYPTION_KEY` is included in the browser bundle in the current design. It can reduce
  accidental plaintext exposure in application storage, but it does not protect against compromise
  of the browser bundle or the key. Do not treat it as a server-only secret.
- Use a separate, randomly generated `JWT_SECRET` for each environment. Keep AWS, Mailgun, and OAuth
  credentials server-side.
- Grant AWS and Mailgun credentials only the permissions required by the deployment.
- Never commit `.env` files, private keys, API keys, or production data.
