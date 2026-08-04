# Swept (swept)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
