# Midpage (midpage)

Midpage is an AI-powered legal research and drafting platform built on its own US legal database of millions of court opinions, statutes, and regulations spanning federal and state jurisdictions. Its developer products expose this corpus through a REST case-law API (semantic, keyword, and hybrid search; opinion retrieval; citator treatments), a Model Context Protocol (MCP) server for AI agents, and direct SQL read-replica access.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/midpage/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/midpage/refs/heads/main/apis.yml)

## Tags

- Legal
- Case Law
- Legal Research
- Search
- AI

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### Midpage Case Law Search API

Full-text keyword search over US court opinions with Lexis/Westlaw-style boolean, phrase, wildcard, and proximity (W/n) operators, plus hybrid search that fuses keyword and semantic results with reciprocal rank fusion. Supports filters by court, jurisdiction, state, publication status, and date, with optional facet breakdowns.

- **Human URL:** [https://midpage-docs.apidocumentation.com/](https://midpage-docs.apidocumentation.com/)
- **Base URL:** `https://app.midpage.ai/api/v1`

#### Tags

- Search
- Case Law
- Keyword
- Hybrid

#### Properties

- [Documentation](https://midpage-docs.apidocumentation.com/)
- [OpenAPI](openapi/midpage-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/midpage.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/midpage.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Midpage Document Retrieval API

Retrieve full opinion data by opinion ID, reporter citation, or docket number, with bulk reads of up to 100 items per request. Optionally include full HTML opinion content and detailed citator treatments via the POST /opinions/get endpoint.

- **Human URL:** [https://midpage-docs.apidocumentation.com/](https://midpage-docs.apidocumentation.com/)
- **Base URL:** `https://app.midpage.ai/api/v1`

#### Tags

- Opinions
- Documents
- Retrieve

#### Properties

- [Documentation](https://midpage-docs.apidocumentation.com/)
- [OpenAPI](openapi/midpage-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/midpage.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/midpage.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Midpage Citations API

Bluebook-style citation lookup and AI-powered citator data returned with retrieved opinions - reporter citations, citation counts, an overall treatment signal (Negative, Caution, Neutral), and per-citing-opinion treatment detail with supporting quotes.

- **Human URL:** [https://midpage-docs.apidocumentation.com/](https://midpage-docs.apidocumentation.com/)
- **Base URL:** `https://app.midpage.ai/api/v1`

#### Tags

- Citations
- Citator
- Treatments

#### Properties

- [Documentation](https://midpage-docs.apidocumentation.com/)
- [OpenAPI](openapi/midpage-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/midpage.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/midpage.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Midpage Semantic Search API

Vector similarity search over court opinions using AI embeddings, ranking results by semantic similarity for conceptual queries. Exposed as the `semantic` mode of the POST /search endpoint and combined with keyword search in `hybrid` mode.

- **Human URL:** [https://midpage-docs.apidocumentation.com/](https://midpage-docs.apidocumentation.com/)
- **Base URL:** `https://app.midpage.ai/api/v1`

#### Tags

- Semantic Search
- Vector
- Embeddings

#### Properties

- [Documentation](https://midpage-docs.apidocumentation.com/)
- [OpenAPI](openapi/midpage-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/midpage.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/midpage.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Midpage MCP Server

Remote Model Context Protocol server (OAuth-authenticated) that gives AI assistants like Claude, ChatGPT, and Perplexity source-grounded legal research tools - search, findInOpinion, analyzeOpinion, and preview docket tools (analyzeDocketReport, analyzeDocketFiling). Versioned tool contracts are served at /mcp/v1, /mcp/v2, and /mcp/v3.

- **Human URL:** [https://www.midpage.ai/integrations](https://www.midpage.ai/integrations)
- **Base URL:** `https://app.midpage.ai/mcp/v3`

#### Tags

- MCP
- Model Context Protocol
- Agents

#### Properties

- [Documentation](https://www.midpage.ai/integrations)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/midpage)
- [Website](https://www.midpage.ai/)
- [Documentation](https://midpage-docs.apidocumentation.com/)
- [Plans](plans/midpage-plans-pricing.yml)
- [Rate Limits](rate-limits/midpage-rate-limits.yml)
- [Fin Ops](finops/midpage-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
