# Deakin University (deakin)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Deakin University is a public research university in Victoria, Australia (Geelong, Warrnambool and Melbourne), ranked #197 in the QS World University Rankings 2025. This repository catalogs Deakin's publicly observable developer and API footprint as an [APIs.json](https://apisjson.org) profile. Deakin does not publish a self-service developer API portal; its confirmed machine-readable surface is research-centric (the figshare-hosted DRO repository with OAI-PMH/REST, a public research Data Portal) plus a Shibboleth/SAML2 SSO identity provider and an active GitHub organization.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/apis.yml
- Run it with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=deakin-api-evangelist&utm_content=repo

## Type

- Index / Consumer / 3rd-Party

## Tags

- Education
- Higher Education
- University
- Research
- Open Data
- Australia

## APIs

- **Deakin Research Online (DRO) OAI-PMH** — research repository hosted on figshare, metadata harvestable via OAI-PMH. Docs: https://info.figshare.com/user-guide/how-to-use-figshares-oai-pmh-service/ — Repository: https://dro.deakin.edu.au/
- **figshare REST API (DRO platform)** — third-party REST API (v2) powering DRO. Docs: https://docs.figshare.com/
- **Deakin Data Portal** — public research data-sharing portal (web-delivered, no documented API confirmed): https://dataportal.deakin.edu.au/
- **Deakin Single Sign-On** — Shibboleth/SAML2 identity provider for federated SSO: https://signon.deakin.edu.au/

## Plans

- [plans/deakin-plans-pricing.yml](plans/deakin-plans-pricing.yml)

## Rate Limits

- [rate-limits/deakin-rate-limits.yml](rate-limits/deakin-rate-limits.yml)

## FinOps

- [finops/deakin-finops.yml](finops/deakin-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.deakin.edu.au/
- GitHub: https://github.com/Deakin
- LinkedIn: https://au.linkedin.com/school/deakin-university/
- Authentication (SSO): https://signon.deakin.edu.au/
- Plans, Rate Limits, FinOps, and Review pointers (see files above)

## Notes

Verification caveats: no first-party documented developer API or public API portal was found for Deakin. The DRO repository host returns a bot-challenge (HTTP 202) to automated clients and is hosted on figshare, whose OAI-PMH and REST APIs are the actual machine-readable surface. The main website (www.deakin.edu.au) returns HTTP 403 to automated fetches due to bot protection but resolves in a browser. The Victorian Marine Data Portal (vmdp.deakin.edu.au) did not resolve during probing. SSO is federated identity infrastructure, not a documented public OAuth/OpenID developer API. No endpoints were fabricated; all entries reflect URLs probed on 2026-06-03.

## Maintainers

- Kin Lane — kin@apievangelist.com
