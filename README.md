# AIB Group (UK) (aib-group-uk)

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

AIB Group (UK) p.l.c. is a UK bank incorporated in Northern Ireland (registered number NI018800, registered office 92 Ann Street, Belfast BT1 3HH), authorised by the Prudential Regulation Authority and regulated by the Financial Conduct Authority and the PRA. It trades as Allied Irish Bank (GB) and Allied Irish Bank (GB) Savings Direct and is the UK banking subsidiary of the Irish AIB Group plc. As one of the CMA9 banks mandated under the UK Competition and Markets Authority's Open Banking order, it runs a public developer portal publishing UK Open Banking APIs conformant to the Open Banking Implementation Entity (OBIE) standards.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/aib-group-uk/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/aib-group-uk/refs/heads/main/apis.yml)

## Tags

- Financial Services
- Banking
- Open Banking
- PSD2
- OBIE
- CMA9
- United Kingdom
- Payments
- Account Information
- Confirmation of Funds
- Northern Ireland

## Timestamps

- **Created:** 2026-07-23
- **Modified:** 2026-07-23

## APIs

### AIB Group (UK) Open Data API

Public, unauthenticated Open Banking Open Data API (v2.2) publishing Allied Irish Bank (GB) product reference data - personal current accounts, business current accounts, and unsecured SME loans - conformant to the OBIE Open Data standard. Confirmed live (HTTP 200, `application/prs.openbanking.opendata.v2.2+json`).

- **Human URL:** [https://developer.aibgb.co.uk/open-data-v2-2-gb/apis](https://developer.aibgb.co.uk/open-data-v2-2-gb/apis)
- **Base URL:** `https://openapi.aibgb.co.uk/open-banking/v2.2`

#### Properties

- [OpenAPI](openapi/aib-group-uk-open-data-openapi.json) — OBIE Open Data standard (shared spec, not an AIB-proprietary contract)
- [Documentation](https://developer.aibgb.co.uk/open-data-v2-2-gb/apis)
- [API Reference](https://developer.aibgb.co.uk/apis)

### AIB Group (UK) Accounts Information API

OBIE Read/Write Account and Transaction Information API (AIS) v4.0 - account details, balances, transactions, standing orders, direct debits, and statements. FAPI-secured via OAuth2/OIDC consent with PSD2 strong customer authentication.

- **Human URL:** [https://developer.aibgb.co.uk/accounts-information-v4-0-gb/apis](https://developer.aibgb.co.uk/accounts-information-v4-0-gb/apis)

### AIB Group (UK) Payments Initiation API

OBIE Read/Write Payment Initiation API (PIS) v4.0 - domestic and scheduled payment initiation. FAPI-secured via OAuth2/OIDC with PSD2 strong customer authentication.

- **Human URL:** [https://developer.aibgb.co.uk/payments-initiation-v4-0-gb/apis](https://developer.aibgb.co.uk/payments-initiation-v4-0-gb/apis)

### AIB Group (UK) Confirmation of Funds API

OBIE Read/Write Confirmation of Funds API (CBPII) v4.0 - yes/no confirmation of fund availability for a specified payment. FAPI-secured via OAuth2/OIDC with PSD2 strong customer authentication.

- **Human URL:** [https://developer.aibgb.co.uk/confirmation-funds-v4-0-gb/apis](https://developer.aibgb.co.uk/confirmation-funds-v4-0-gb/apis)

### AIB Group (UK) Variable Recurring Payments API

OBIE Read/Write Variable Recurring Payments (VRP) API v4.0, including sweeping. FAPI-secured via OAuth2/OIDC with PSD2 strong customer authentication.

- **Human URL:** [https://developer.aibgb.co.uk/variable-recurring-payments-v4-0-gb/apis](https://developer.aibgb.co.uk/variable-recurring-payments-v4-0-gb/apis)

### AIB Group (UK) Dynamic Client Registration API

OBIE Dynamic Client Registration API v3.2 - programmatic client registration using OBIE/eIDAS certificates.

- **Human URL:** [https://developer.aibgb.co.uk/dynamic-client-registration-api-v3-2-gb/apis](https://developer.aibgb.co.uk/dynamic-client-registration-api-v3-2-gb/apis)

### AIB Group (UK) Credit Cards Information API

Credit Cards Information API providing access to credit card account information under the Open Banking consent model.

- **Human URL:** [https://developer.aibgb.co.uk/credit-cards-information-gb/apis](https://developer.aibgb.co.uk/credit-cards-information-gb/apis)

### AIB Group (UK) Event Notification Subscription API

OBIE Event Notification Subscription API v4.0 for managing subscriptions to Read/Write event notifications.

- **Human URL:** [https://developer.aibgb.co.uk/event-notification-subscription-api-v4-0-gb/apis](https://developer.aibgb.co.uk/event-notification-subscription-api-v4-0-gb/apis)

### AIB Group (UK) Aggregated Event Polling API

OBIE Aggregated Event Polling API v4.0 for polling aggregated event notifications.

- **Human URL:** [https://developer.aibgb.co.uk/aggregated-event-polling-api-v4-0-gb/apis](https://developer.aibgb.co.uk/aggregated-event-polling-api-v4-0-gb/apis)

### AIB Group (UK) FCA Service Metrics (BCA) API

FCA Service Metrics API for Business Current Accounts, publishing FCA-required availability and performance metrics.

- **Human URL:** [https://developer.aibgb.co.uk/fca-service-metrics-bca-gb/apis](https://developer.aibgb.co.uk/fca-service-metrics-bca-gb/apis)

## Common Properties

- [Website](https://www.aibgb.co.uk/)
- [Developer Portal](https://developer.aibgb.co.uk/)
- [Documentation](https://developer.aibgb.co.uk/apis)
- [Support](https://developer.aibgb.co.uk/faq-page)
- [Terms of Service](https://developer.aibgb.co.uk/site-legal-notice-gb)
- [Privacy Policy](https://developer.aibgb.co.uk/developer-portal-privacy-statement-GB)
- [Compliance](https://developer.aibgb.co.uk/fca-service-metrics-bca-gb/apis)
- [LinkedIn](https://www.linkedin.com/company/aib)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
