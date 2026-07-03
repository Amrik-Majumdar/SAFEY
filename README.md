# SAFEY

SAFEY is a browser-based safety application focused on discreet access, local privacy controls, and offline-friendly safety planning. It was built by Amrik Majumdar and Atiksh Gupta.

SAFEY won the 2025 Congressional App Challenge for Virginia's 11th District as "SAFEY, Safety Assessment and Resource Platform." The public Congressional App Challenge listing credits Amrik Majumdar and Atiksh Gupta, and describes the project as a Progressive Web App designed to support people experiencing domestic violence through risk assessment, safety planning, and access to critical resources.

The application is designed around sensitive user contexts, so the repository emphasizes discreet interaction patterns, local-first storage, clear user control, and careful handling of personal information.

## Recognition

- 2025 Congressional App Challenge winner, Virginia's 11th District
- Listed by the Congressional App Challenge as "SAFEY, Safety Assessment and Resource Platform"
- Built by Amrik Majumdar and Atiksh Gupta
- Public-safe personal repository prepared for portfolio review

Official references:

- [Congressional App Challenge winner article](https://www.congressionalappchallenge.us/25-va11/)
- [2025 Congressional App Challenge winners list](https://www.congressionalappchallenge.us/2025-winners/)
- [U.S. House Congressional App Challenge listing](https://www.house.gov/educators-and-students/congressional-app-challenge/Virginia)

## What This Project Shows

- Mobile-oriented safety interface
- Stealth and disguise flows for sensitive contexts
- Trusted-contact and alert-message workflows
- Local storage and encrypted local settings
- Service worker and offline behavior
- Cloudflare Worker proxy structure for optional chatbot support
- Public-safe repository cleanup with local cache files excluded
- A civic-technology project with externally verified competition recognition

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

The project includes disguise-mode behavior, safety-check flows, resource lists, trusted-contact message preparation, local event storage, lockout handling, and offline support through a service worker. These pieces are organized as browser modules so the core experience can run without a heavy backend.

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

## Attribution and Source

This repository was prepared from the collaborative SAFEY codebase for public portfolio review. The project should be credited as:

```text
Made by Amrik Majumdar and Atiksh Gupta
```

The source used for this cleanup came from:

```text
ag2027/SAFEY_1
```

Only this personal repository was modified during cleanup.

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
