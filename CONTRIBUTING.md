# Contributing to Mailhub

Issues and pull requests are welcome. Before opening a pull request:

1. Keep the change focused and explain its user-visible impact.
2. Run the checks relevant to the repository you changed. For backend changes, run
   `npm run lint`, `npm run typecheck`, `npm test -- --runInBand`,
   `npm run test:e2e -- --runInBand`, and `npm run build`. For frontend changes, run that
   repository's documented lint and build commands.
3. Do not include secrets or real email addresses in commits, tests, or screenshots.

Please report security vulnerabilities through the private channel in [SECURITY.md](SECURITY.md)
instead of opening a public issue.
