# OrderPilot

OrderPilot is a standalone, mobile-friendly prototype for post-purchase support operations at small online retailers.

## Current prototype
- Overview dashboard with case counts
- Customer case register with search and status filter
- Delivery follow-up view
- Returns and complaints view
- Create/update demo cases
- CSV export
- Fictional sample records only
- Browser-local demo persistence

## Run locally
Open `index.html` in a modern browser. No build step or paid service is required for this static prototype.

## Cloudflare Pages
This repository is intended to hold the OrderPilot application source. The existing `live-hq` Cloudflare Pages project is **not currently connected to this repository**.

Do not change the existing Pages project's Git integration to point here unless the Live HQ site source and deployment strategy have first been accounted for. A Pages project serves a complete deployment; simply pointing it at this standalone repository would replace the currently deployed site rather than automatically mount OrderPilot beneath it.

To host OrderPilot at `/orderpilot` within the existing Live HQ deployment, the deployment must include both the Live HQ site and the OrderPilot assets, or use a deliberately configured separate service/route. Confirm the current Live HQ build output and routing before production integration.

## Production blockers
This is a UI prototype, not a production customer-support system.
- No authentication or authorisation
- No server-side database
- No retailer tenant isolation
- No audit log
- No POPIA-ready personal-data handling
- No email, WhatsApp, courier or commerce integrations

Do not enter real customer information. Use fictional demo data only until secure server-side authentication, database access controls, tenant isolation, retention policies and lawful processing arrangements are implemented and tested.
