# EZLynx (ezlynx)

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

EZLynx is an insurance agency platform combining real-time comparative rating, an agency management system (AMS), and CRM for independent property and casualty (P&C) insurance agencies. It has been part of **Applied Systems** since March 2021. EZLynx offers enterprise API solutions that let agencies and technology partners push and pull data, create and update applicants, contacts, prospects, and opportunities, create policy headers, retrieve policy and quote-result data, and drive high-volume automated quoting through the **EZLynx Rating Engine** and **Quoting Automation Services (QAS)**. An event-driven layer emits webhook notifications in XML or JSON when platform data changes.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/ezlynx/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/ezlynx/refs/heads/main/apis.yml)

## Access Model — Partner / Enterprise-Gated

EZLynx does **not** run a public, self-serve developer program. There is:

- No public developer portal or open API key signup
- No publicly published API pricing (enterprise, contact sales)
- No openly hosted, machine-readable API reference

Public product and integration material indicates the API is **REST over HTTPS** with **OAuth 2.0** authentication and **XML or JSON** payloads, plus an **event-driven webhook** layer. A Postman-hosted collection exists as reference, but working credentials, the base URL, and the full endpoint surface are provided under a partner or enterprise agreement. Prospective integrators contact EZLynx / Applied Systems sales.

Because of this, the APIs listed below are **honestly modeled** from EZLynx's public product pages, integration write-ups, and the referenced Postman collection description — **not** copied from a published open reference. The concrete request paths and base URL are gated, so no specific endpoint paths have been fabricated (`endpointsModeled: true` in `review.yml`).

## Tags

- Insurance
- InsurTech
- Comparative Rating
- Agency Management System
- CRM
- Quoting
- Property and Casualty
- Applied Systems

## Timestamps

- **Created:** 2026-07-10
- **Modified:** 2026-07-10

## APIs (Logical, Modeled)

### EZLynx Applicants and Contacts API

Create and update applicants, contacts, prospects, and opportunities in the EZLynx management system and CRM so external lead-capture, marketing, and onboarding tools stay in sync without rekeying data.

- **Human URL:** [https://www.ezlynx.com/products/ezlynx-api-solutions/](https://www.ezlynx.com/products/ezlynx-api-solutions/)

### EZLynx Rating Engine API

Submit applicant and risk data to the EZLynx Rating Engine for high-volume automated comparative quoting and retrieve quote results. Surfaces the backend behind Quoting Automation Services (QAS) and EZLynx Data Bridge.

- **Human URL:** [https://www.ezlynx.com/products/ezlynx-api-solutions/](https://www.ezlynx.com/products/ezlynx-api-solutions/)

### EZLynx Policies API

Create policy headers and retrieve policy information from the EZLynx management system for downstream accounting, servicing, and reporting.

- **Human URL:** [https://www.ezlynx.com/products/ezlynx-api-solutions/](https://www.ezlynx.com/products/ezlynx-api-solutions/)

### EZLynx Management System Data API

Read supporting management-system data — email templates, documents, and user data — so integrated applications can reuse an agency's content and org structure.

- **Human URL:** [https://www.ezlynx.com/products/ezlynx-api-solutions/](https://www.ezlynx.com/products/ezlynx-api-solutions/)

### EZLynx Events and Webhooks API

Consume EZLynx's event-driven layer — webhook notifications delivered in XML or JSON when platform data changes (new clients, policy updates) — to trigger downstream automation. Delivery is one-way HTTP webhook callouts, **not** a public WebSocket.

- **Human URL:** [https://www.ezlynx.com/products/ezlynx-api-solutions/](https://www.ezlynx.com/products/ezlynx-api-solutions/)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/ezlynx)
- [Website](https://www.ezlynx.com)
- [Documentation](https://www.ezlynx.com/products/ezlynx-api-solutions/)
- [API Reference (Postman)](https://documenter.getpostman.com/view/17108315/UVXjHahb)
- [Sign Up / Enterprise](https://www.ezlynx.com/solutions/enterprise/)
- [Blog](https://www.ezlynx.com/blog/)

## WebSocket Review

EZLynx does **not** expose a documented public WebSocket API. Its own public surface is REST over HTTPS (OAuth 2.0) plus one-way HTTP webhook events; both are partner/enterprise-gated. See `review.yml`.

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
