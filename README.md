# Mono (mono-co)

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

Mono is an African open-banking platform that lets businesses access bank and financial data and collect recurring payments through a single API. The Mono REST API at api.withmono.com covers account linking (Connect), transactions, statements, identity, income, and balance, plus DirectPay one-time payments and Direct Debit mandates, secured with a mono-sec-key header.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/apis.yml)

## Tags

- Open Banking
- Financial Data
- Payments
- Direct Debit
- Africa

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### Account Linking and Auth

Initiate Mono Connect account linking and exchange the returned code for a persistent account id, instantiating the bank-data connection used by all downstream account endpoints.

- **Human URL:** [https://docs.mono.co/docs/financial-data/overview](https://docs.mono.co/docs/financial-data/overview)
- **Base URL:** `https://api.withmono.com`

#### Tags

- Account Linking
- Authorization
- Connect

#### Properties

- [Documentation](https://docs.mono.co/docs/financial-data/integration-guide)
- [API Reference](https://docs.mono.co/api/bank-data/authorisation/initiate-account-linking)
- [OpenAPI](openapi/mono-co-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mono-co.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mono-co.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Account Information

Retrieve account details and a near-real-time account balance for a linked account by its account id.

- **Human URL:** [https://docs.mono.co/docs/financial-data/overview](https://docs.mono.co/docs/financial-data/overview)
- **Base URL:** `https://api.withmono.com`

#### Tags

- Account Information
- Balance
- Connect

#### Properties

- [Documentation](https://docs.mono.co/docs/financial-data/overview)
- [API Reference](https://docs.mono.co/api/bank-data/accounts/details)
- [OpenAPI](openapi/mono-co-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mono-co.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mono-co.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Transactions and Statements

Pull money-in and money-out transactions with date, type, and narration filters, and retrieve a customer's bank statement in JSON or PDF form for a linked account.

- **Human URL:** [https://docs.mono.co/api/bank-data/transactions](https://docs.mono.co/api/bank-data/transactions)
- **Base URL:** `https://api.withmono.com`

#### Tags

- Transactions
- Statements
- Financial Data

#### Properties

- [Documentation](https://docs.mono.co/api/bank-data/transactions)
- [API Reference](https://docs.mono.co/api/bank-data/transactions)
- [OpenAPI](openapi/mono-co-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mono-co.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mono-co.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Identity and Income

Verify a linked account holder's identity (name, phone, date of birth, BVN) and retrieve income signals including estimated salary and income sources derived from financial data.

- **Human URL:** [https://docs.mono.co/api/bank-data/accounts/identity](https://docs.mono.co/api/bank-data/accounts/identity)
- **Base URL:** `https://api.withmono.com`

#### Tags

- Identity
- Income
- KYC

#### Properties

- [Documentation](https://docs.mono.co/api/bank-data/accounts/identity)
- [API Reference](https://docs.mono.co/api/bank-data/accounts/income)
- [OpenAPI](openapi/mono-co-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mono-co.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mono-co.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### DirectPay Payments

Initiate one-time bank-to-bank DirectPay payments and verify their status, returning a hosted payment link for the customer to authorize.

- **Human URL:** [https://docs.mono.co/docs/payments/overview](https://docs.mono.co/docs/payments/overview)
- **Base URL:** `https://api.withmono.com`

#### Tags

- Payments
- DirectPay
- Bank Transfer

#### Properties

- [Documentation](https://docs.mono.co/docs/payments/overview)
- [API Reference](https://docs.mono.co/api/directpay/initiate)
- [OpenAPI](openapi/mono-co-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mono-co.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mono-co.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Direct Debit and Mandates

Create customers, set up fixed or variable direct-debit mandates on a customer's bank account, run a confirmation-of-funds balance inquiry, and debit an authorized mandate for recurring collections.

- **Human URL:** [https://docs.mono.co/docs/payments/direct-debit/overview](https://docs.mono.co/docs/payments/direct-debit/overview)
- **Base URL:** `https://api.withmono.com`

#### Tags

- Direct Debit
- Mandates
- Recurring Payments

#### Properties

- [Documentation](https://docs.mono.co/docs/payments/direct-debit/overview)
- [API Reference](https://docs.mono.co/api/direct-debit/mandate/initiate-mandate-authorisation)
- [OpenAPI](openapi/mono-co-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mono-co.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mono-co.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Webhooks

Server-to-server webhook callbacks for Connect account events (connected, updated, reauthorisation required, unlinked) and payment events (DirectPay and Direct Debit success and failure), delivered as POST requests with a shared event/data/timestamp payload.

- **Human URL:** [https://docs.mono.co/docs/webhooks](https://docs.mono.co/docs/webhooks)
- **Base URL:** `https://api.withmono.com`

#### Tags

- Webhooks
- Events
- Notifications

#### Properties

- [Documentation](https://docs.mono.co/docs/webhooks)
- [API Reference](https://docs.mono.co/docs/payments/direct-debit/webhook-events)
- [OpenAPI](openapi/mono-co-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mono-co.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mono-co.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/withmono)
- [LinkedIn](https://www.linkedin.com/company/mono-hq)
- [Website](https://mono.co)
- [Documentation](https://docs.mono.co)
- [Plans](plans/mono-co-plans-pricing.yml)
- [Rate Limits](rate-limits/mono-co-rate-limits.yml)
- [Fin Ops](finops/mono-co-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
