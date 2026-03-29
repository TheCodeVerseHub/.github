# Security Policy

We take security seriously across all TheCodeVerseHub repositories.

## Reporting a vulnerability

Please **do not** open a public GitHub issue for security reports.

Instead, email: **contact@thecodeversehub.tech**

Include:

- A clear description of the issue and affected repository
- Steps to reproduce (or a proof of concept)
- Impact assessment (what can an attacker do?)
- Any suggested fix or mitigation

If the vulnerability involves a secret leak (tokens/keys), rotate the secret
immediately and mention what was rotated.

## Response expectations

- **Acknowledgement:** typically within 72 hours
- **Triage:** we’ll confirm scope/impact and propose next steps
- **Fix:** timing depends on severity and maintainer availability

If you need a coordinated disclosure timeline, mention it in your email.

## Supported repositories

Because this org contains multiple early-stage projects, support level varies.
We will prioritize:

- Projects actively deployed (bots / website)
- Projects that process user data (even minimal identifiers)

## Security notes for contributors

- Never commit `.env` files or tokens
- Prefer minimal permissions for bot tokens and OAuth apps
- Keep dependencies updated and pinned where possible
