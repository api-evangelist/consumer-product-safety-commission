# Consumer Product Safety Commission (consumer-product-safety-commission)

The U.S. Consumer Product Safety Commission (CPSC) is the federal agency responsible for protecting the public from unreasonable risks of injury or death associated with consumer products such as toys, household items, electronics, and furniture. CPSC publishes a public, unauthenticated Recalls Retrieval Web Service that exposes recall records (with products, hazards, manufacturers, retailers, distributors, importers, and remedies) in JSON or XML, plus the SaferProducts.gov OData service for incident-report data accessed by application key.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/consumer-product-safety-commission/refs/heads/main/apis.yml)

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
- **Modified:** 2026-04-29

## APIs

### CPSC Recalls API
Public REST web service that returns CPSC recall records published on cpsc.gov. Supports case-insensitive wildcard search across recall number, date, product type, hazard, country, manufacturer, retailer, importer, distributor, and UPC. Output is available as JSON or XML and the API requires no authentication.

**Human URL:** [https://www.cpsc.gov/Recalls/CPSC-Recalls-Application-Program-Interface-API-Information](https://www.cpsc.gov/Recalls/CPSC-Recalls-Application-Program-Interface-API-Information)

**Base URL:** `https://www.saferproducts.gov/RestWebServices`

#### Properties

- [Documentation](https://www.cpsc.gov/Recalls/CPSC-Recalls-Application-Program-Interface-API-Information)
- [Programmers Guide (PDF)](https://cpsc.gov/s3fs-public/RecallRetrievalWebServicesProgrammersGuide20180917.pdf)
- [OpenAPI](openapi/cpsc-recalls-openapi.yml)

### SaferProducts.gov OData API
OData web service exposing publicly published consumer product incident-report data submitted through SaferProducts.gov. Authenticated with a basic-auth header where the registered application key is sent as the username (no password).

**Human URL:** [https://www.saferproducts.gov/FAQs/FrequentlyAskedQuestions11](https://www.saferproducts.gov/FAQs/FrequentlyAskedQuestions11)

**Base URL:** `https://www.saferproducts.gov/WebApi/Cpsc.Cpsrms.Web.Api.svc`

#### Properties

- [Documentation](https://www.saferproducts.gov/FAQs/FrequentlyAskedQuestions11)
- [OData Metadata](https://www.saferproducts.gov/WebApi/Cpsc.Cpsrms.Web.Api.svc/$metadata)

## Common Properties

- [Website](https://www.cpsc.gov/)
- [Recalls](https://www.cpsc.gov/Recalls)
- [Data](https://www.cpsc.gov/Data)
- [SaferProducts.gov](https://www.saferproducts.gov/)
- [Public Search](https://www.saferproducts.gov/PublicSearch)
- [Programmers Guide](https://cpsc.gov/s3fs-public/RecallRetrievalWebServicesProgrammersGuide20180917.pdf)
- [Privacy Policy](https://www.cpsc.gov/Newsroom/Privacy-and-Security-Statement)
- [JSON-LD Context](json-ld/consumer-product-safety-commission-context.jsonld)
- [Recall JSON Schema](json-schema/cpsc-recall-schema.json)
- [Spectral Ruleset](rules/consumer-product-safety-commission-rules.yml)
- [Naftiko Capabilities](capabilities/consumer-product-safety-commission-capabilities.yml)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
