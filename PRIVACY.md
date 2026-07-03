# Privacy Policy

Last updated: July 2026

SAFEY is designed as a privacy-conscious safety planning Progressive Web App. The core app is intended to keep safety-planning information local to the user's browser whenever possible.

This policy describes the public repository and intended app behavior. It is not a substitute for a deployment-specific privacy policy if the app is hosted, modified, or connected to additional services.

## Information The Core App May Store Locally

Depending on how the app is used, the browser may store:

- safety-plan entries
- trusted-contact information entered by the user
- risk assessment state
- stealth and lockout settings
- local event or check-in history
- decoy or disguise-mode settings

This local data should remain on the user's device unless a user chooses to send a message, place a call, use an external resource, or enable an externally connected feature.

## External Services

Some features may open external websites, phone apps, SMS apps, email clients, or optional chatbot/proxy services. Those services may have their own privacy practices. Review any external service before enabling or deploying it.

## Data Not To Commit

This repository should not contain:

- real trusted-contact information
- safety plans from real users
- user logs
- API keys
- worker account caches
- private `.env` files
- deployment credentials

## Safety Context

Because this project is intended for sensitive situations, any deployment should be reviewed carefully for privacy, security, device access, browser storage behavior, and the risk that an unsafe person could inspect the device.

## Contact

Questions about this public repository can be directed to: majumdar.amrik@gmail.com
