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

Deakin University is a public research university in Victoria, Australia (Geelong, Warrnambool and Melbourne). This repository catalogs Deakin's publicly observable programmable footprint as an [APIs.json](https://apisjson.org) profile, with an explicit operator recorded on every surface. Deakin publishes no developer portal and no OpenAPI. Its one institution-operated machine-readable contract is the SAML 2.0 metadata it serves for a Shibboleth identity provider it runs on its own APNIC address space; everything else that is callable under a Deakin name belongs to a platform Deakin buys.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/apis.yml
- Run it with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=deakin-api-evangelist&utm_content=repo

## Type

- Index / Consumer / 3rd-Party — `x-type: university`, `x-category: Public Research University`

## Tags

- Education
- Higher Education
- University
- Research
- Australia
- Victoria
- Identity Federation
- Research Repository
- Research Data
- Learning Management

## Surfaces, by operator

A university is a federation of buyers, not a producer. Each entry below carries an `x-operator` in
`apis.yml` saying who runs the thing it describes.

**Institution-operated**

- **Deakin University SAML 2.0 Identity Provider** — self-served EntityDescriptor at https://signon.deakin.edu.au/idp/shibboleth (HTTP 200, application/xml, 4,826 bytes), on 128.184.0.0/16 (APNIC netname DEAKINUNIVERSITY) under a Deakin-procured DigiCert certificate. Archived at [identity-federation/deakin-idp-saml-metadata.xml](identity-federation/deakin-idp-saml-metadata.xml).
- **Deakin Data Portal** — https://dataportal.deakin.edu.au/, on Deakin's own address space and registered in the AAF as a Shibboleth SP, but every path returns an F5/Shape JavaScript challenge, so no contract could be read from it.

**Tenant — Deakin's data, someone else's contract**

- **Deakin Research Online (DRO)** — figshare (dro.deakin.edu.au → proxy-eu-01.figshare.com).
- **CloudDeakin** — D2L Brightspace (d2l.deakin.edu.au → deakin.brightspace.com); its keyless Valence version manifest is the only JSON API answering on any deakin.edu.au host.
- **Federated SSO** — AAF Rapid IdP (aaf.deakin.edu.au → idp-cname.aaf.edu.au on Amazon).
- **Library discovery** — Ex Libris (library.deakin.edu.au → EXLIBRIS-20-1).
- **DataCite repository ARDCX.DEAKIN** — prefix 10.26187, 4,597 DOIs.
- **Crossref member 8935** — prefix 10.21153, 1,303 works.

## Identity Federation

- [identity-federation/deakin-identity-federation.yml](identity-federation/deakin-identity-federation.yml)
- [identity-federation/deakin-idp-saml-metadata.xml](identity-federation/deakin-idp-saml-metadata.xml)

## Conformance (Kin Score `education` regime)

- [conformance/deakin-conformance.yml](conformance/deakin-conformance.yml) — conformant on `saml`, `shibboleth`, `datacite` and `crossref`; `lti` and `oai-pmh` are present only through tenant and vendor platforms and are not credited to Deakin.

## Plans

- [plans/deakin-plans-pricing.yml](plans/deakin-plans-pricing.yml)

## Rate Limits

- [rate-limits/deakin-rate-limits.yml](rate-limits/deakin-rate-limits.yml)

## FinOps

- [finops/deakin-finops.yml](finops/deakin-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-08-30

## Common Properties

- Website: https://www.deakin.edu.au/
- Open Data: https://dataportal.deakin.edu.au/
- Research Repository: https://dro.deakin.edu.au/
- Library: https://www.deakin.edu.au/library
- Course Catalog: https://www.deakin.edu.au/study/find-a-course
- AI Policy: https://www.deakin.edu.au/about-deakin/why-deakin/generative-artificial-intelligence
- AI Tooling: https://www.deakin.edu.au/students/study-support/study-resources/artificial-intelligence
- GitHub: https://github.com/Deakin
- LinkedIn: https://au.linkedin.com/school/deakin-university/
- Blog: https://blogs.deakin.edu.au/
- Identity Federation, Conformance, Domain Security, Plans, Rate Limits, FinOps and Review pointers (see files above)

## Notes

**This profile was corrected on 2026-08-30.** The June 2026 version credited Deakin with eleven APIs.
Every one of them was a tag-split of a single figshare contract — `info.title` "Figshare altmetric …
API", `info.contact` "Figshare Support", `servers` `https://api.figshare.com/v2` — and eleven other
institutions in this cohort ship the same document. Ten OpenAPIs, the pristine source spec, and the
43 artifacts derived from them (collections, JSON Schema, JSON Structure, examples, JSON-LD,
vocabulary, rulesets, authentication, scopes, agentic-access, capability map) were removed file by
file. The figshare relationship is kept, as a tenant surface, because it is a real institutional
fact — but the contract is figshare's and belongs in figshare's profile.

Verification caveats: operator was settled by DNS, whois and TLS certificate procurement, never by
hostname. The deakin.edu.au web estate (www, blogs, dataportal, handbook, research) sits behind
F5/Shape bot protection which answers automated clients with HTTP 403 or a 200 carrying a JavaScript
challenge body — including `blogs.deakin.edu.au/wp-json/`, so no WordPress REST surface is claimed.
`library.deakin.edu.au` timed out from our vantage point. `vmdp.deakin.edu.au` still does not
resolve. `api.deakin.edu.au` returns 404. No endpoints were fabricated; every entry reflects a URL
probed on 2026-08-30 and recorded with its status code in [review.yml](review.yml).

## Maintainers

- Kin Lane — kin@apievangelist.com
