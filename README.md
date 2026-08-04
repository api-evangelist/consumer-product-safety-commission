# Consumer Product Safety Commission (consumer-product-safety-commission)

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

The U.S. Consumer Product Safety Commission (CPSC) is the federal agency responsible for protecting the public from unreasonable risks of injury or death associated with consumer products such as toys, household items, electronics, and furniture. CPSC publishes a public, unauthenticated Recalls Retrieval Web Service that exposes recall records (with products, hazards, manufacturers, retailers, distributors, importers, and remedies) in JSON or XML, plus the SaferProducts.gov OData service for incident-report data accessed by application key.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/consumer-product-safety-commission/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/consumer-product-safety-commission/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

- Consumer Protection
- Federal Government
- Hazards
- Open Data
- Product Safety
- Recalls

## Timestamps

- **Created:** 2024-12-25
- **Modified:** 2026-05-19

## APIs

### CPSC Recalls API

Public REST web service that returns CPSC recall records published on cpsc.gov. Supports case-insensitive wildcard search across recall number, date, product type, hazard, country, manufacturer, retailer, importer, distributor, and UPC. Output is available as JSON or XML and the API requires no authentication.

- **Human URL:** [https://www.cpsc.gov/Recalls/CPSC-Recalls-Application-Program-Interface-API-Information](https://www.cpsc.gov/Recalls/CPSC-Recalls-Application-Program-Interface-API-Information)
- **Base URL:** `https://www.saferproducts.gov/RestWebServices`

#### Tags

- JSON
- Open Data
- Recalls
- REST
- XML

#### Properties

- [Documentation](https://www.cpsc.gov/Recalls/CPSC-Recalls-Application-Program-Interface-API-Information)
- [Reference](https://cpsc.gov/s3fs-public/RecallRetrievalWebServicesProgrammersGuide20180917.pdf)
- [OpenAPI](openapi/cpsc-recalls-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cpsc-recalls.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cpsc-recalls.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### SaferProducts.gov OData API

OData web service exposing publicly published consumer product incident-report data submitted through SaferProducts.gov. Authenticated with a basic-auth header where the registered application key is sent as the username (no password).

- **Human URL:** [https://www.saferproducts.gov/FAQs/FrequentlyAskedQuestions11](https://www.saferproducts.gov/FAQs/FrequentlyAskedQuestions11)
- **Base URL:** `https://www.saferproducts.gov/WebApi/Cpsc.Cpsrms.Web.Api.svc`

#### Tags

- Incident Reports
- OData
- Open Data

#### Properties

- [Documentation](https://www.saferproducts.gov/FAQs/FrequentlyAskedQuestions11)
- [Reference](https://www.saferproducts.gov/WebApi/Cpsc.Cpsrms.Web.Api.svc/$metadata)
- [Postman Collection](collections/cpsc-recalls.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cpsc-recalls.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://www.cpsc.gov/)
- [Recalls](https://www.cpsc.gov/Recalls)
- [Data](https://www.cpsc.gov/Data)
- [Safer Products.gov](https://www.saferproducts.gov/)
- [Public  Search](https://www.saferproducts.gov/PublicSearch)
- [Programmers  Guide](https://cpsc.gov/s3fs-public/RecallRetrievalWebServicesProgrammersGuide20180917.pdf)
- [Privacy Policy](https://www.cpsc.gov/Newsroom/Privacy-and-Security-Statement)
- [Terms of Service](https://www.cpsc.gov/Newsroom/Privacy-and-Security-Statement)
- [JSON-LD](json-ld/consumer-product-safety-commission-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON Schema](json-schema/cpsc-recall-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Spectral Rules](rules/consumer-product-safety-commission-rules.yml) — [Spectral](https://docs.stoplight.io/docs/spectral)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
