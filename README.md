# Bank Australia (bank-australia)

Bank Australia is a customer-owned (mutual) bank headquartered in Collingwood, Victoria, tracing its origins to the 1957 CSIRO Co-operative Credit Society and formed through the merger of more than 70 credit unions and co-operatives (via mecu and bankmecu) before adopting the Bank Australia name in 2015. As an APRA-regulated authorised deposit-taking institution (ADI) and a certified B Corporation, it is owned by its customers rather than shareholders and is known for responsible, fossil-fuel-free lending. Under Australia's Consumer Data Right (CDR / Open Banking), Bank Australia operates as a data holder and exposes a public, unauthenticated Product Reference Data (PRD) API conforming to the Data Standards Body (DSB) Consumer Data Standards.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/bank-australia/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/bank-australia/refs/heads/main/apis.yml)

## Tags

- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Australia
- Mutual Bank

## Timestamps

- **Created:** 2026-07-20
- **Modified:** 2026-07-20

## APIs

### Bank Australia CDR Product Reference Data API

Public, unauthenticated Product Reference Data (PRD) endpoints under the Consumer Data Right. Serves `GET /banking/products` and `GET /banking/products/{productId}` at the CDS public base, returning machine-readable product, fee, rate, and eligibility data for Bank Australia's deposit, credit card, and lending products. Requests require the mandatory CDS `x-v` version header. The contract is the shared DSB Consumer Data Standards Banking OpenAPI (OpenAPI 3.0.3), not a bank-proprietary specification.

- **Human URL:** [https://www.bankaust.com.au/support/open-banking/developer/](https://www.bankaust.com.au/support/open-banking/developer/)
- **Base URL:** `https://public.cdr.bankaust.com.au/cds-au/v1`

#### Tags

- CDR
- Open Banking
- Product Reference Data
- Banking
- Public

#### Properties

- [Documentation](https://www.bankaust.com.au/support/open-banking/developer/)
- [API Reference](https://consumerdatastandardsaustralia.github.io/standards/#cdr-banking-api_get-products)
- [OpenAPI](https://consumerdatastandardsaustralia.github.io/standards/includes/swagger/cds_banking.json) — shared DSB Consumer Data Standards Banking OpenAPI 3.0.3 (not bank-proprietary)

## Common Properties

- [Website](https://www.bankaust.com.au/)
- [Developer Portal](https://www.bankaust.com.au/support/open-banking/developer/)
- [Documentation](https://www.bankaust.com.au/support/open-banking)
- [LinkedIn](https://au.linkedin.com/company/bankaust)
- [Blog](https://www.bankaust.com.au/blog)
- [Privacy Policy](https://www.bankaust.com.au/support/website-security-and-privacy-statement)
- [Terms of Service](https://www.bankaust.com.au/support/disclosures)
- [Support](https://www.bankaust.com.au/support)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
