# SAFEY

SAFEY is a browser-based safety application focused on discreet access, local privacy controls, and offline-friendly safety planning. The project was adapted from the upstream `ag2027/SAFEY_1` source into this personal repository for public portfolio review.

The application is designed around sensitive user contexts, so the repository emphasizes local storage, clear user control, and careful handling of personal information.

## What This Project Shows

- Mobile-oriented safety interface
- Stealth and disguise flows for sensitive contexts
- Trusted-contact and alert-message workflows
- Local storage and encrypted local settings
- Service worker and offline behavior
- Cloudflare Worker proxy structure for optional chatbot support
- Public-safe repository cleanup with local cache files excluded

## Repository Structure

```text
.
├── index.html              Main application page
├── app.js                  Primary application logic
├── service-worker.js       Offline caching behavior
├── manifest.json           PWA metadata
├── js/
│   ├── crypto-utils.js
│   ├── stealth-controller.js
│   ├── stealth-settings.js
│   ├── unlock-handler.js
│   ├── trusted-contacts.js
│   └── other interface modules
├── worker/
│   ├── index.js            Optional worker proxy
│   └── wrangler.toml
└── README.md
```

## Technical Approach

SAFEY is built as a client-side web application with modular JavaScript files. The browser handles the interface, local safety-plan data, trusted-contact flows, and stealth interactions. Sensitive settings are stored locally, with encryption helpers used for parts of the local data model.

The worker folder contains optional proxy code for chatbot-style support. Worker account caches and local Wrangler metadata should not be committed.

## Local Usage

Because the app is static, it can be served locally with any simple web server:

```powershell
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Privacy and Safety Notes

- Core safety-planning behavior is designed to stay local to the browser.
- SMS and phone actions open the device's native apps; the user still decides whether to send or call.
- Optional chatbot support depends on external service configuration and should be reviewed before use.
- This repository should not contain real trusted-contact data, user logs, API keys, worker account caches, or private environment files.

## Upstream Source

This personal repo was refreshed from:

```text
ag2027/SAFEY_1
```

Only this personal fork was modified during cleanup.

## Limitations

- Browser safety tools should be tested carefully on target devices.
- The public repository is not a substitute for professional safety planning.
- Optional chatbot support requires separate configuration.
- Local storage and browser APIs behave differently across browsers and devices.

## Future Improvements

- Add screenshots of the major flows.
- Add accessibility testing notes.
- Document worker deployment steps without including account-specific cache files.
- Add a small test checklist for stealth mode, lockout behavior, and offline caching.
