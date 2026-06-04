# Deakin University (deakin)

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
