# Pixieset

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Pixieset is an all-in-one photography business platform - client galleries, a store for print/digital sales, a website builder, a mobile gallery app, and Studio Manager (CRM, booking, invoicing, contracts, questionnaires) - used by hundreds of thousands of photographers. Pixieset does not publish a public or partner developer API, does not run a developer program, and has no self-serve API keys or OAuth signup; there is no official API reference, SDK, or webhook system for third parties. The product itself is powered internally by two session-cookie-authenticated web APIs (a Studio API at studio.pixieset.com/api/v1 for business management and a Gallery API at galleries.pixieset.com/api/v1 for gallery delivery and e-commerce) that Pixieset's own web app calls, and which an independent developer has reverse-engineered and published as unofficial, unaffiliated documentation (111+ endpoints). This entry documents that real access model honestly - no public API exists, and the endpoint shapes below are modeled from that third-party reverse-engineering effort, not from any Pixieset-published reference - treat them as unverified and subject to change or removal without notice.

**Areas:** Photography · Client Galleries · Studio Management · CRM · Booking · Invoicing · Contracts

## Pixieset on APIs.io

Everything profiled for Pixieset is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/pixieset/](https://apis.io/providers/pixieset/)** — or go straight to one of the APIs or properties below.

### APIs (5)

- [Pixieset Clients API](https://apis.io/apis/pixieset/pixieset-clients-api/) — Client and lead CRM records.
- [Pixieset Collections API](https://apis.io/apis/pixieset/pixieset-collections-api/) — Gallery collections, access, and downloads.
- [Pixieset Contracts API](https://apis.io/apis/pixieset/pixieset-contracts-api/) — Contracts and contract templates.
- [Pixieset Invoices API](https://apis.io/apis/pixieset/pixieset-invoices-api/) — Invoices and payments.
- [Pixieset Sessions API](https://apis.io/apis/pixieset/pixieset-sessions-api/) — Bookable session types, scheduling, and availability.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Pixieset Agentic Access](https://apis.io/agentic-access/pixieset/pixieset-agentic-access/)

#### Collections (5)

Postman and Open Collection request collections.

- [Pixieset Studio & Gallery API (Modeled, Unofficial) Clients API](https://apis.io/collections/pixieset/open-pixieset-clients-api/)
- [Pixieset Studio & Gallery API (Modeled, Unofficial) Clients Collections API](https://apis.io/collections/pixieset/open-pixieset-collections-api/)
- [Pixieset Studio & Gallery API (Modeled, Unofficial) Clients Contracts API](https://apis.io/collections/pixieset/open-pixieset-contracts-api/)
- [Pixieset Studio & Gallery API (Modeled, Unofficial) Clients Invoices API](https://apis.io/collections/pixieset/open-pixieset-invoices-api/)
- [Pixieset Studio & Gallery API (Modeled, Unofficial) Clients Sessions API](https://apis.io/collections/pixieset/open-pixieset-sessions-api/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Pixieset Authentication](https://apis.io/security/pixieset/pixieset-authentication/)
- [Pixieset Domain Security](https://apis.io/security/pixieset/pixieset-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Pixieset Plans Pricing](https://apis.io/plans/pixieset/pixieset-plans-pricing/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://pixieset.com)
- [Documentation](https://help.pixieset.com/hc/en-us)

## API Evangelist rating

**Kin Score 21.5** — emerging · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 66.1 |
| Contract quality | 35.3 |
| Contract governance | 0.0 |
| Operational transparency | 0.0 |
| Developer ergonomics | 28.6 |
| Access clarity | 7.9 |

**Agent readiness 17.3** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 11.8** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/pixieset/](https://apis.io/providers/pixieset/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Pixieset: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/pixieset/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
