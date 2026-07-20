---
name: Look up Bank Australia banking products
description: >-
  Retrieve Bank Australia's public product reference data (deposit, credit card,
  and lending products with fees, rates, and eligibility) via the Consumer Data
  Right Product Reference Data API. No authentication required.
api: cds_banking.json (Consumer Data Standards Banking, OpenAPI 3.0.3)
base_url: https://public.cdr.bankaust.com.au/cds-au/v1
operations: [listBankingProducts, getBankingProductDetail]
---

# Look up Bank Australia banking products

This skill uses Bank Australia's **public, unauthenticated** CDR Product
Reference Data API. There is no API key or OAuth flow for these endpoints — the
only mandatory input is the CDS `x-v` version header.

## Rules

- Always send the request header `x-v: 3` (integer CDS API version). Omitting it
  returns `400 urn:au-cds:error:cds-all:Header/Missing`; an unsupported value
  returns `406 urn:au-cds:error:cds-all:Header/UnsupportedVersion`. Read the
  served version back from the `x-v` response header.
- These are GET-only, read-only operations — no idempotency key, no write state.
- Optionally send/propagate `x-fapi-interaction-id` for request tracing; the
  server echoes it (or generates one).

## Steps

1. **List products** — call `listBankingProducts`:
   `GET /banking/products?page-size=25` with header `x-v: 3`.
   Page with `page` and `page-size` (max 1000); read `meta.totalRecords`,
   `meta.totalPages`, and `links.next`. Requesting a page beyond range returns
   `422 urn:au-cds:error:cds-all:Field/InvalidPage`; a bad `page-size` returns
   `400 urn:au-cds:error:cds-all:Field/InvalidPageSize`.

2. **Get one product** — take a `productId` from the list and call
   `getBankingProductDetail`:
   `GET /banking/products/{productId}` with header `x-v: 3`.
   An unknown id returns `404 urn:au-cds:error:cds-all:Resource/Invalid`.

3. **Handle errors** — all failures use the CDS error envelope
   `{ "errors": [ { "code": "urn:au-cds:error:cds-all:...", "title": ..., "detail": ... } ] }`
   (see `errors/bank-australia-problem-types.yml`).

## Notes

Account and transaction data (Consumer Data Sharing) is a separate, authenticated
surface governed by the CDR security profile (OAuth2/OIDC + mTLS + FAPI) and is
NOT reachable through these public product endpoints.
