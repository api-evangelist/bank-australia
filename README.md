# Bank Australia (bank-australia)

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
