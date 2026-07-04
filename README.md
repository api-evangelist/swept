# Swept (swept)

Swept ([sweptworks.com](https://sweptworks.com)) is workforce management software for commercial cleaning and janitorial businesses. It combines scheduling, GPS-verified time tracking and payroll reporting, mobile crew messaging, quality inspections, supply requests, client portals, and one-time work order management, founded in 2014 in Halifax, Nova Scotia.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/swept/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/swept/refs/heads/main/apis.yml)

## API Access Model — No Public Developer API

> **Honest status:** As of this catalog entry (2026-07-04), Swept does **not** publish a documented, self-serve public or partner developer API. This entry is an intentional stub. No API definitions, OpenAPI specs, rate limits, or FinOps files are asserted, because none are publicly documented.

What the research confirmed:

- **No developer portal, no API reference, no API key or OAuth signup, no published OpenAPI/Swagger specification, and no webhook documentation** on sweptworks.com or in the [Swept Support Center](https://knowledge.sweptworks.com/knowledge/resources) knowledge base (Getting Started, Scheduling, Time Tracking, Inspections, Supplies, Clients, Mobile App, Operations).
- The only documented outbound data path is a **one-way QuickBooks Online payroll sync** - manually activated per account by a Swept Customer Success Manager, syncing approved payroll entries from Swept into QuickBooks. Changes made in QuickBooks do not sync back. This is an internal, account-by-account integration, not a self-serve developer API. See [How do I sync my account with QuickBooks?](https://knowledge.sweptworks.com/knowledge/how-do-i-sync-my-account-with-quickbooks)
- Swept does not integrate directly with payroll providers beyond QuickBooks; instead it offers CSV/PDF export of time data for use with any payroll system.
- The [Swept GitHub organization](https://github.com/sweptworks) contains only **take-home coding-challenge repositories** used for engineering hiring (`react-flask-takehome`, `poker-takehome`, `python-react-takehome`) plus two unrelated forks (`nameko-examples`, `alpine-android`). There is **no first-party Swept API client, SDK, or OpenAPI specification** published anywhere.
- Swept's public "App Store" page lists product features and mobile apps, not third-party integrations or a marketplace of API-connected apps.

If you need to move data into or out of Swept today, the practical paths are: (1) use the web app and iOS/Android mobile apps directly, (2) export payroll data as CSV/PDF for any payroll system, (3) ask a Customer Success Manager to activate the one-way QuickBooks Online sync, or (4) contact Swept directly ([contact@sweptworks.com](mailto:contact@sweptworks.com)) about a custom data integration.

## Logical Product Areas (not documented APIs)

For reference only - these are the functional areas a Swept API *would* cover if one were published. **No endpoints are documented or modeled here** (`endpointsModeled: none`):

- **Employees / Crew** - cleaner profiles, roles, permissions
- **Locations / Sites** - client sites, geofences, service schedules
- **Time Tracking** - GPS clock in/out, mobile and IVR call-in, break compliance
- **Scheduling** - shift assignment, one-time work orders
- **Inspections** - quality checks with photo and note capture
- **Supplies** - supply requests and fulfillment
- **Clients** - client portal, direct client messaging
- **Payroll** - payroll reporting and export, one-way QuickBooks Online sync

## Tags

- Janitorial
- Commercial Cleaning
- Workforce Management
- Scheduling
- Time Tracking
- Payroll
- Inspections
- Field Service
- No Public API

## Timestamps

- **Created:** 2026-07-04
- **Modified:** 2026-07-04

## Pricing

Swept publishes three cumulative tiers priced by **number of managed locations**, not per employee, starting at a 1-15 location band: **Launch** (starting at $30/month - scheduling, time tracking, payroll export, no-show alerts), **Optimize** (starting at $150/month - adds break compliance, geofenced messaging, inspections), and **Scale** (starting at $225/month - adds travel time, profitability reporting, supply management, client portal, one-time work orders). Annual billing saves up to 20%. There is no separate API/developer pricing tier because there is no public API. See [Compare Plans](https://sweptworks.com/compare-plans) and [plans/swept-plans-pricing.yml](plans/swept-plans-pricing.yml).

## Common Properties

- [Website](https://sweptworks.com)
- [LinkedIn](https://www.linkedin.com/company/swept)
- [GitHub Organization](https://github.com/sweptworks)
- [Documentation (Support Center)](https://knowledge.sweptworks.com/knowledge/resources)
- [Plans](plans/swept-plans-pricing.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
