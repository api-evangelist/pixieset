# Pixieset (pixieset)

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

Pixieset is an all-in-one photography business platform - client galleries, a store for print/digital sales, a website builder, a mobile gallery app, and Studio Manager (CRM, booking, invoicing, contracts, questionnaires) - used by hundreds of thousands of photographers.

**Access model:** Pixieset does not publish a public or partner developer API, does not run a developer program, and has no self-serve API keys or OAuth signup; there is no official API reference, SDK, or webhook system for third parties. The product itself is powered internally by two session-cookie-authenticated web APIs (a Studio API at `studio.pixieset.com/api/v1` for business management and a Gallery API at `galleries.pixieset.com/api/v1` for gallery delivery and e-commerce) that Pixieset's own web app calls, and which an independent developer has reverse-engineered and published as unofficial, unaffiliated documentation (111+ endpoints, [trozz.github.io/pixieset-api-docs](https://trozz.github.io/pixieset-api-docs/)). This entry documents that real access model honestly: no public API exists, and the endpoint shapes captured here are modeled from that third-party reverse-engineering effort, not from any Pixieset-published reference - treat them as unverified and subject to change or removal without notice. Pixieset also has no official Zapier or Make.com integration, and its own public status page ("Our Public API" at pixieset.instatus.com/public-api) monitors uptime only, with no link to developer documentation.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/pixieset/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/pixieset/refs/heads/main/apis.yml)

## Tags

- Photography
- Client Galleries
- Studio Management
- CRM
- Booking
- Invoicing
- Contracts
- No Public API

## Timestamps

- **Created:** 2026-07-04
- **Modified:** 2026-07-04

## APIs

### Pixieset Studio Clients & CRM API

Internal client relationship management surface of Pixieset's own Studio web app - list, search, retrieve, and update clients and leads (id prefix `cl_`), their address info, notes, associated galleries, and documents. Not a Pixieset-published API; endpoint shapes are modeled from unofficial third-party reverse-engineering documentation and are unverified against Pixieset's current implementation.

- **Human URL:** [https://trozz.github.io/pixieset-api-docs/docs/studio-api/clients](https://trozz.github.io/pixieset-api-docs/docs/studio-api/clients)
- **Base URL:** `https://studio.pixieset.com/api/v1`

#### Tags

- Clients
- CRM
- Leads

#### Properties

- [Documentation](https://trozz.github.io/pixieset-api-docs/docs/studio-api/overview)
- [API Reference](https://trozz.github.io/pixieset-api-docs/docs/studio-api/clients)
- [OpenAPI](openapi/pixieset-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Pixieset Studio Sessions & Booking API

Internal session-type and booking surface used by the Studio web app - define bookable session types (id prefix `set_`) with duration, location, pricing, and payment methods, check day/month availability, manage schedules and interval overrides, and list booked sessions and pending inquiries. Not a Pixieset-published API; modeled from unofficial reverse-engineering documentation, unverified against Pixieset's current implementation.

- **Human URL:** [https://trozz.github.io/pixieset-api-docs/docs/studio-api/sessions](https://trozz.github.io/pixieset-api-docs/docs/studio-api/sessions)
- **Base URL:** `https://studio.pixieset.com/api/v1`

#### Tags

- Sessions
- Bookings
- Scheduling

#### Properties

- [API Reference](https://trozz.github.io/pixieset-api-docs/docs/studio-api/sessions)
- [OpenAPI](openapi/pixieset-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Pixieset Studio Invoices & Payments API

Internal invoicing and payment surface used by the Studio web app - list and retrieve invoices (id prefix `in_`) and line items in the smallest currency unit, read per-invoice and per-client payment records (id prefix `ip_`) including processor/transaction fees and card/PayPal details, invoice summaries and currency totals, and disputed-payment counts. Not a Pixieset-published API; modeled from unofficial reverse-engineering documentation, unverified against Pixieset's current implementation.

- **Human URL:** [https://trozz.github.io/pixieset-api-docs/docs/studio-api/invoices](https://trozz.github.io/pixieset-api-docs/docs/studio-api/invoices)
- **Base URL:** `https://studio.pixieset.com/api/v1`

#### Tags

- Invoices
- Payments
- Billing

#### Properties

- [API Reference](https://trozz.github.io/pixieset-api-docs/docs/studio-api/invoices)
- [OpenAPI](openapi/pixieset-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Pixieset Studio Contracts API

Internal contracts surface used by the Studio web app - list and retrieve client contracts (id prefix `co_`) with rendered HTML content, due dates, status, and multi-party signature records, plus manage reusable contract templates (id prefix `ct_`) with HTML body, `{{variable}}` placeholders, signer configuration, and due-day/reminder settings. Not a Pixieset-published API; modeled from unofficial reverse-engineering documentation, unverified against Pixieset's current implementation.

- **Human URL:** [https://trozz.github.io/pixieset-api-docs/docs/studio-api/contracts](https://trozz.github.io/pixieset-api-docs/docs/studio-api/contracts)
- **Base URL:** `https://studio.pixieset.com/api/v1`

#### Tags

- Contracts
- Documents
- E-Signature

#### Properties

- [API Reference](https://trozz.github.io/pixieset-api-docs/docs/studio-api/contracts)
- [OpenAPI](openapi/pixieset-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Pixieset Gallery Collections & Delivery API

Internal gallery-delivery surface used by Pixieset's client galleries product - manage collections that group galleries of photos and videos, control password protection, expiry, and per-client access, list collection clients and visitor emails, and track photo/video downloads, sharing links, and client favorites for the built-in print/digital-sales store. Not a Pixieset-published API; modeled from unofficial reverse-engineering documentation, unverified against Pixieset's current implementation.

- **Human URL:** [https://trozz.github.io/pixieset-api-docs/docs/gallery-api/overview](https://trozz.github.io/pixieset-api-docs/docs/gallery-api/overview)
- **Base URL:** `https://galleries.pixieset.com/api/v1`

#### Tags

- Galleries
- Collections
- Client Delivery
- E-Commerce

#### Properties

- [Documentation](https://trozz.github.io/pixieset-api-docs/docs/gallery-api/overview)
- [API Reference](https://trozz.github.io/pixieset-api-docs/docs/gallery-api/collections)
- [OpenAPI](openapi/pixieset-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/pixieset)
- [Website](https://pixieset.com)
- [Documentation](https://help.pixieset.com/hc/en-us)
- [Plans](plans/pixieset-plans-pricing.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
