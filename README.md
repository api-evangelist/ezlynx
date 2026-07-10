# EZLynx (ezlynx)

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
