# SOAX

SOAX provides enterprise-grade proxy infrastructure and web data extraction APIs for developers and data teams. With 155M+ residential IPs, 33M+ mobile IPs, and 300K+ datacenter IPs across 195+ countries, SOAX enables web scraping, CAPTCHA bypass, geo-targeted data collection, and anti-bot circumvention at scale.

## APIs

### SOAX Web Data API

Extract fully rendered web content from any public website with automatic CAPTCHA bypass, JavaScript rendering, and anti-bot protection.

- **Documentation:** https://docs.soax.com/
- **Getting Started:** https://helpcenter.soax.com/en/articles/11297318-getting-started-with-soax-web-data-api
- **OpenAPI Spec:** [openapi/soax-web-data-api-openapi.yml](openapi/soax-web-data-api-openapi.yml)

**Endpoints:**
- `POST /v2/webdata/fetch-content` — Fetch rendered HTML, screenshots, XHR, or Markdown
- `POST /v2/webdata/serp` — Extract search engine result pages
- `POST /v2/webdata/ecommerce` — Extract product pricing and inventory data

### SOAX Proxy Management API

Programmatically manage proxy packages, IP whitelists, and geo-targeting options.

- **Documentation:** https://helpcenter.soax.com/en/collections/3470979-api
- **OpenAPI Spec:** [openapi/soax-proxy-management-api-openapi.yml](openapi/soax-proxy-management-api-openapi.yml)

**Endpoints:**
- `GET /v1/account/package/{key}/ip-list` — List whitelisted IPs
- `POST /v1/account/package/{key}/update-ip` — Whitelist an IP address
- `POST /v1/account/package/{key}/detach-ip` — Remove a whitelisted IP
- `GET /v1/geo/cities` — List available cities for geo-targeting
- `GET /v1/geo/regions` — List available regions/states
- `GET /v1/geo/carriers` — List available mobile carriers
- `GET /v1/geo/isps` — List available WiFi ISPs

## Artifacts

| Type | File |
|------|------|
| OpenAPI (Web Data API) | [openapi/soax-web-data-api-openapi.yml](openapi/soax-web-data-api-openapi.yml) |
| OpenAPI (Proxy Management) | [openapi/soax-proxy-management-api-openapi.yml](openapi/soax-proxy-management-api-openapi.yml) |
| JSON Schema | [json-schema/soax-fetch-request-schema.json](json-schema/soax-fetch-request-schema.json) |
| JSON Structure | [json-structure/soax-fetch-request-structure.json](json-structure/soax-fetch-request-structure.json) |
| JSON-LD Context | [json-ld/soax-context.jsonld](json-ld/soax-context.jsonld) |
| Spectral Rules | [rules/soax-rules.yml](rules/soax-rules.yml) |
| Vocabulary | [vocabulary/soax-vocabulary.yml](vocabulary/soax-vocabulary.yml) |
| Example: Fetch Content | [examples/soax-fetch-content-example.json](examples/soax-fetch-content-example.json) |

## Capabilities

### Workflows

| Capability | File | Description |
|-----------|------|-------------|
| Data Collection | [capabilities/data-collection.yaml](capabilities/data-collection.yaml) | Unified web scraping, SERP extraction, e-commerce data, and proxy management (8 MCP tools) |

### Shared Definitions

| API | File |
|-----|------|
| SOAX Web Data API | [capabilities/shared/soax-web-data-api.yaml](capabilities/shared/soax-web-data-api.yaml) |
| SOAX Proxy Management API | [capabilities/shared/soax-proxy-management-api.yaml](capabilities/shared/soax-proxy-management-api.yaml) |

## Links

- **Website:** https://soax.com/
- **Documentation:** https://docs.soax.com/
- **Help Center:** https://helpcenter.soax.com/
- **Pricing:** https://soax.com/pricing
- **Sign Up:** https://soax.com/get-started
- **Blog:** https://soax.com/blog/

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
