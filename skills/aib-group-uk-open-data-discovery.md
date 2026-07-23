---
name: Discover AIB Group (UK) branches, ATMs, and products via Open Data
description: >-
  Query the public, unauthenticated AIB Group (UK) Open Banking Open Data API
  (v2.2) to retrieve Allied Irish Bank (GB) branches, ATMs, and product
  reference data (personal current accounts, business current accounts,
  unsecured SME loans, commercial credit cards). No credentials required.
api: openapi/aib-group-uk-open-data-openapi.json
base_url: https://openapi.aibgb.co.uk/open-banking/v2.2
operations:
  - GET /branches
  - GET /atms
  - GET /personal-current-accounts
  - GET /business-current-accounts
  - GET /unsecured-sme-loans
  - GET /commercial-credit-cards
---

# Discover AIB Group (UK) branches, ATMs, and products

The AIB Group (UK) Open Data API is **public and unauthenticated** — no OAuth,
no API key. It is served under the OBIE Open Data v2.2 standard and returns
`application/prs.openbanking.opendata.v2.2+json`.

## Prerequisites

- Base URL: `https://openapi.aibgb.co.uk/open-banking/v2.2`
- No authentication.
- Set an `Accept` header of `application/prs.openbanking.opendata.v2.2+json`
  (or `application/json`).

## Steps

1. **Pick the resource** you need:
   - `GET /branches` — physical branch locations, services, accessibility.
   - `GET /atms` — ATM locations and supported services.
   - `GET /personal-current-accounts` — PCA products, rates, fees, eligibility.
   - `GET /business-current-accounts` — BCA products and terms.
   - `GET /unsecured-sme-loans` — unsecured SME loan products.
   - `GET /commercial-credit-cards` — commercial credit card products.

2. **Issue the GET.** Each response is a `Meta` block
   (`LastUpdated`, `TotalResults`, `Agreement`, `Licence`, `TermsOfUse`)
   wrapping a `Brand[]` array; each brand carries a `BrandName` and the relevant
   product/asset array (see `data-model/aib-group-uk-data-model.yml`).

3. **Use conditional requests** to poll efficiently: send `If-None-Match` with
   the previously returned `Etag` (or `If-Modified-Since`) and treat `304 Not
   Modified` as "no change". Respect `Cache-Control` (`max-age`).

4. **Handle errors** per `errors/aib-group-uk-problem-types.yml`:
   `400` bad request, `408` timeout, `429` too many requests (back off and slow
   your polling), `500` server error, `503` temporarily unavailable (retry with
   backoff).

## Notes

- This Open Data surface is product/location reference data only. Account,
  balance, transaction, and payment data live in the FAPI-secured Read/Write
  APIs, which require OBIE OAuth2/OIDC consent and PSD2 SCA — see
  `authentication/aib-group-uk-authentication.yml`.
- Rate limits: keep polling modest; `429` means slow down.
