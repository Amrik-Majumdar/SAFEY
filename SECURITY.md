# Security Policy

Last updated: July 2026

SAFEY is a sensitive-context safety application. Security concerns should be reported privately, especially if they involve local data exposure, stealth-mode bypasses, lockout behavior, trusted-contact flows, worker configuration, or accidental publication of private files.

## Reporting A Security Issue

Please report security concerns privately by email:

**majumdar.amrik@gmail.com**

Include:

- a summary of the issue
- affected file, page, or feature
- steps to reproduce
- screenshots or logs if they do not expose private data

## Public-Safe Rules

- Do not commit API keys, tokens, worker account caches, or `.env` files.
- Do not commit real trusted-contact data or safety plans.
- Review local storage behavior before deployment.
- Test stealth, lockout, and exit flows on target devices.
- Review optional chatbot/proxy configuration before enabling it.

## Safety Note

Security issues in this project can have real personal-safety implications. Please avoid public issue reports that disclose a bypass or data exposure before it can be reviewed.
