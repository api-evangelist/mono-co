# Mono (mono-co)

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
