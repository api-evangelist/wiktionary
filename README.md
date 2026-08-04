# Wiktionary (wiktionary)

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

Wiktionary is the free, collaborative multilingual dictionary project of the Wikimedia Foundation, the dictionary sibling of Wikipedia. Programmatic access is exposed through the MediaWiki Action API at en.wiktionary.org/w/api.php, the older Wikimedia REST API at en.wiktionary.org/api/rest_v1/ (which provides Wiktionary-specific endpoints like /page/definition/{term}), and the newer MediaWiki Core REST API at en.wiktionary.org/w/rest.php. All Wiktionary content is licensed CC BY-SA 4.0 (and GFDL) and hosted by the Wikimedia Foundation.

**URL:** [Visit APIs.json URL](https://en.wiktionary.org/w/api.php)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Dictionaries, Open Source, Wikimedia, MediaWiki, Linguistics, Open Data, Public APIs

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-30

## APIs

### MediaWiki Action API (Wiktionary)
The MediaWiki Action API is the original Wikimedia query/edit API exposed at /w/api.php on every Wikimedia project. For Wiktionary it provides access to wikitext definitions, page parsing, full-text search, and OpenSearch suggestions. Actions include action=query (prop=wikitext, prop=extracts, prop=revisions, list=search), action=parse (rendered wikitext HTML and section trees), action=opensearch (suggestions), and action=expandtemplates. Supports both GET and POST with format=json|xml.

**Human URL:** [https://en.wiktionary.org/w/api.php](https://en.wiktionary.org/w/api.php)

**Base URL:** `https://en.wiktionary.org/w/api.php`

#### Tags:

 - Dictionaries, MediaWiki, Wikitext

#### Properties

- [Documentation](https://en.wiktionary.org/w/api.php)
- [APIReference](https://www.mediawiki.org/wiki/API:Main_page)
- [GettingStarted](https://www.mediawiki.org/wiki/API:Tutorial)
- [Authentication](https://www.mediawiki.org/wiki/API:Authentication)
- [RateLimits](https://www.mediawiki.org/wiki/API:Etiquette)
- [Sandbox](https://en.wiktionary.org/wiki/Special:ApiSandbox)
- [OpenAPI](openapi/wiktionary-mediawiki-action-api-openapi-original.yml)
- [JSONLD](json-ld/wiktionary-mediawiki-action-api-context.jsonld)

#### Artifact Counts

- **JSONSchema**: 12
- **JSONStructure**: 12
- **Example**: 12
- **NaftikoCapability**: 4

#### Naftiko Capabilities

- [Wiktionary MediaWiki Action API — ExpandTemplates](capabilities/mediawiki-action-api-expandtemplates.yaml) — 1 MCP tool
- [Wiktionary MediaWiki Action API — OpenSearch](capabilities/mediawiki-action-api-opensearch.yaml) — 1 MCP tool
- [Wiktionary MediaWiki Action API — Parse](capabilities/mediawiki-action-api-parse.yaml) — 1 MCP tool
- [Wiktionary MediaWiki Action API — Query](capabilities/mediawiki-action-api-query.yaml) — 4 MCP tools

### Wikimedia REST API (Wiktionary)
The Wikimedia REST API (the older "RESTBase" service) is hosted per project at /api/rest_v1/ and includes Wiktionary-specific endpoints such as /page/definition/{term} which returns multilingual structured definitions parsed from wikitext, plus generic page endpoints (/page/html/{title}, /page/summary/{title}, /page/title/{title}, /page/mobile-html/{title}) and Parsoid transform endpoints (/transform/html/to/wikitext, /transform/wikitext/to/html, /transform/wikitext/to/lint). Capped at ~200 req/s, requires a unique User-Agent.

**Human URL:** [https://en.wiktionary.org/api/rest_v1/](https://en.wiktionary.org/api/rest_v1/)

**Base URL:** `https://en.wiktionary.org/api/rest_v1`

#### Tags:

 - Dictionaries, Definitions, REST, Parsoid

#### Properties

- [Documentation](https://en.wiktionary.org/api/rest_v1/)
- [APIReference](https://en.wiktionary.org/api/rest_v1/?spec)
- [Sandbox](https://en.wiktionary.org/api/rest_v1/?doc)
- [RateLimits](https://api.wikimedia.org/wiki/Rate_limits)
- [OpenAPI](openapi/wiktionary-rest-api-openapi-original.yml)
- [JSONLD](json-ld/wiktionary-rest-api-context.jsonld)

#### Artifact Counts

- **JSONSchema**: 10
- **JSONStructure**: 10
- **Example**: 10
- **NaftikoCapability**: 3

#### Naftiko Capabilities

- [Wiktionary Wikimedia REST API — Definition](capabilities/rest-api-definition.yaml) — 1 MCP tool
- [Wiktionary Wikimedia REST API — Page Content](capabilities/rest-api-page-content.yaml) — 4 MCP tools
- [Wiktionary Wikimedia REST API — Transform](capabilities/rest-api-transform.yaml) — 3 MCP tools

### MediaWiki Core REST API (Wiktionary)
The newer MediaWiki Core REST API is exposed at /w/rest.php on every wiki. It offers a smaller, more streamlined surface than the Action API for fetching pages, history, search, files, and revisions. On Wiktionary it serves the same content as the Action API in a more developer-friendly JSON shape. Endpoints include /v1/page/{title}, /v1/page/{title}/html, /v1/page/{title}/history, /v1/search/page, /v1/search/title, /v1/file/{title}.

**Human URL:** [https://en.wiktionary.org/w/rest.php/v1](https://en.wiktionary.org/w/rest.php/v1)

**Base URL:** `https://en.wiktionary.org/w/rest.php`

#### Tags:

 - Dictionaries, REST, MediaWiki Core

#### Properties

- [Documentation](https://www.mediawiki.org/wiki/API:REST_API)
- [APIReference](https://www.mediawiki.org/wiki/API:REST_API/Reference)
- [Sandbox](https://en.wiktionary.org/wiki/Special:RestSandbox)
- [OpenAPI](openapi/wiktionary-core-rest-api-openapi-original.yml)
- [JSONLD](json-ld/wiktionary-core-rest-api-context.jsonld)

#### Artifact Counts

- **JSONSchema**: 10
- **JSONStructure**: 10
- **Example**: 10
- **NaftikoCapability**: 4

#### Naftiko Capabilities

- [Wiktionary MediaWiki Core REST API — File](capabilities/core-rest-api-file.yaml) — 1 MCP tool
- [Wiktionary MediaWiki Core REST API — History](capabilities/core-rest-api-history.yaml) — 3 MCP tools
- [Wiktionary MediaWiki Core REST API — Page](capabilities/core-rest-api-page.yaml) — 3 MCP tools
- [Wiktionary MediaWiki Core REST API — Search](capabilities/core-rest-api-search.yaml) — 2 MCP tools

## Common Properties

- [Website](https://en.wiktionary.org/)
- [DeveloperPortal](https://api.wikimedia.org/)
- [Documentation](https://www.mediawiki.org/wiki/API)
- [APIReference](https://www.mediawiki.org/wiki/API:Main_page)
- [GitHubOrganization (Wikimedia GitHub Mirror)](https://github.com/wikimedia)
- [GitHubOrganization (Wikimedia Gerrit (Canonical))](https://gerrit.wikimedia.org/)
- [Authentication](https://api.wikimedia.org/wiki/Authentication)
- [RateLimits](https://api.wikimedia.org/wiki/Rate_limits)
- [TermsOfService](https://foundation.wikimedia.org/wiki/Terms_of_Use)
- [PrivacyPolicy](https://foundation.wikimedia.org/wiki/Privacy_policy)
- [Pricing (Free (CC BY-SA 4.0))](https://en.wiktionary.org/wiki/Wiktionary:About)
- [StatusPage](https://www.wikimediastatus.net/)
- [Blog](https://diff.wikimedia.org/)
- [Support](https://www.mediawiki.org/wiki/Project:Support_desk)
- [ChangeLog](https://www.mediawiki.org/wiki/MediaWiki_1.42)
- [SDK (Pywikibot (Python))](https://www.mediawiki.org/wiki/Manual:Pywikibot)
- [SDK (mwclient (Python))](https://github.com/mwclient/mwclient)
- [SDK (mwn (TypeScript/Node.js))](https://github.com/siddharthvp/mwn)
- [SDK (nodemw (Node.js))](https://github.com/nodemw/nodemw)
- [SDK (wikitools3 (Python))](https://github.com/dmwilcox/wikitools3)
- [SDK (wiki-java (Java))](https://github.com/MER-C/wiki-java)
- [SDK (jwiki (Java))](https://github.com/Fastily/jwiki)
- [SDK (mediawiki-api-base (PHP))](https://github.com/addshore/mediawiki-api-base)
- [SDK (mediawiki-ruby-api (Ruby))](https://github.com/wikimedia/mediawiki-ruby-api)
- [SDK (mwparserfromhell (Python wikitext parser))](https://github.com/sadnub/mwparserfromhell)
- [CLI (Pywikibot CLI)](https://www.mediawiki.org/wiki/Manual:Pywikibot)
- [Tools (Wikidata Query Service)](https://github.com/Professor-G/MediaWikiAPI)
- [GitHubRepository (MediaWiki Core)](https://github.com/wikimedia/mediawiki)
- [GitHubRepository (RESTBase)](https://github.com/wikimedia/restbase)
- [GitHubRepository (Parsoid (Wikitext ↔ HTML))](https://github.com/wikimedia/parsoid)
- [GitHubRepository (Pywikibot)](https://github.com/wikimedia/pywikibot)
- [SpectralRules](rules/wiktionary-spectral-rules.yml)
- [Vocabulary](vocabulary/wiktionary-vocabulary.yml)

## Features

| Name | Description |
|------|-------------|
| Multilingual Definitions | /page/definition/{term} returns dictionary entries broken down by source language, part of speech, definitions, and usage examples in structured JSON. |
| Wikitext Access | action=query&prop=wikitext returns raw wikitext for any page, enabling clients to build their own parsers and extractors. |
| Rendered HTML | /page/html/{title} and action=parse return Parsoid-generated HTML suitable for direct rendering in client apps. |
| OpenSearch Suggestions | action=opensearch implements the OpenSearch suggestions protocol so Wiktionary can power autocomplete in any search UI. |
| Full-Text Search | action=query&list=search and /v1/search/page expose the same ElasticSearch-backed full-text search Wiktionary uses internally. |
| Page Revisions and History | Both APIs expose full revision history, supporting time-travel reads and change-detection workflows. |
| Wikitext ↔ HTML Transforms | Parsoid /transform/* endpoints convert between wikitext and HTML round-trip-safely, useful for visual editors and bots. |
| OAuth 2.0 and BotPasswords | Authenticated calls support OAuth 2.0 (via api.wikimedia.org), legacy OAuth 1.0a, and BotPassword scoped credentials. |
| CC BY-SA 4.0 License | All Wiktionary content can be reused for any purpose with attribution and share-alike, including in commercial AI training corpora. |

## Use Cases

| Name | Description |
|------|-------------|
| Dictionary Apps | Embed definitions, etymologies, pronunciations, and translations directly into mobile or desktop dictionary apps. |
| Language-Learning Tools | Power vocabulary lookups, flashcards, and reading-assistance browser extensions for learners of any language. |
| NLP and Linguistics Datasets | Use bulk wikitext dumps and the definition API to build morphology, inflection, and word-sense datasets for NLP research. |
| Translation Memory | Mine cross-language Wiktionary translation tables to seed bilingual dictionaries and translation memories. |
| Spell-Checkers and Tokenizers | Use the OpenSearch and search endpoints to validate word existence and segment text in tokenizers. |
| AI Grounding and RAG | Retrieve authoritative definitions to ground LLM responses about word meaning, etymology, and usage. |
| Crossword and Game Generation | Generate clues, anagrams, and puzzle answers from Wiktionary's definitions and word lists. |
| Linguistic Research | Query etymologies, declensions, pronunciations, and historical usage across hundreds of languages. |

## Integrations

| Name | Description |
|------|-------------|
| Wikipedia | Shares infrastructure, accounts, and most APIs with Wikipedia; both run on MediaWiki under the Wikimedia Foundation. |
| Wikidata | Wiktionary lexemes are increasingly linked to structured Wikidata lexeme entities (Lexeme namespace, Q-IDs, L-IDs). |
| Wikimedia Commons | Pronunciation audio files and images embedded in Wiktionary pages live on Commons and are reachable via the same APIs. |
| Pywikibot | The reference bot framework for automated edits, dumps, and maintenance scripts against Wiktionary. |
| Wikimedia Enterprise | Commercial high-volume snapshots of Wikimedia content (Wikipedia first, with broader project coverage expanding); useful when REST rate limits are insufficient. |
| Toolforge | Wikimedia-hosted PaaS for community tools that consume the Wiktionary APIs at scale without bringing your own infrastructure. |
| Hugging Face Datasets | Pre-processed Wiktionary dumps are available on Hugging Face for immediate use in ML training pipelines. |

## Solutions

| Name | Description |
|------|-------------|
| Free Public APIs | The MediaWiki Action API, Wikimedia REST API, and MediaWiki Core REST API are all free to use without registration, subject to the 200 req/s shared limit and User-Agent requirement. |
| Bulk Dumps | dumps.wikimedia.org provides full XML and SQL exports of every Wikimedia project, refreshed at least monthly; the preferred channel for whole-corpus processing. |
| Wikimedia Enterprise | Paid SLA-backed snapshots and streaming APIs for commercial reusers who need throughput, freshness, or attribution guarantees beyond what the free APIs provide. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [wiktionary-core-rest-api-openapi-original.yml](openapi/wiktionary-core-rest-api-openapi-original.yml)
- [wiktionary-mediawiki-action-api-openapi-original.yml](openapi/wiktionary-mediawiki-action-api-openapi-original.yml)
- [wiktionary-rest-api-openapi-original.yml](openapi/wiktionary-rest-api-openapi-original.yml)

### JSON Schema (32 files)

See [`json-schema/`](json-schema/) for all extracted component schemas.

### JSON Structure (32 files)

See [`json-structure/`](json-structure/) for JSON Structure conversions of the schemas.

### JSON-LD Contexts

- [wiktionary-core-rest-api-context.jsonld](json-ld/wiktionary-core-rest-api-context.jsonld)
- [wiktionary-mediawiki-action-api-context.jsonld](json-ld/wiktionary-mediawiki-action-api-context.jsonld)
- [wiktionary-rest-api-context.jsonld](json-ld/wiktionary-rest-api-context.jsonld)

### Examples (32 files)

See [`examples/`](examples/) for one realistic JSON example per schema.

## Capabilities

Self-contained Naftiko capabilities — one file per OpenAPI tag, each declaring both a REST and an MCP adapter inline.

| Capability | APIs | MCP Tools |
|------------|------|-----------|
| [Wiktionary MediaWiki Core REST API — File](capabilities/core-rest-api-file.yaml) | core-rest-api | 1 |
| [Wiktionary MediaWiki Core REST API — History](capabilities/core-rest-api-history.yaml) | core-rest-api | 3 |
| [Wiktionary MediaWiki Core REST API — Page](capabilities/core-rest-api-page.yaml) | core-rest-api | 3 |
| [Wiktionary MediaWiki Core REST API — Search](capabilities/core-rest-api-search.yaml) | core-rest-api | 2 |
| [Wiktionary MediaWiki Action API — ExpandTemplates](capabilities/mediawiki-action-api-expandtemplates.yaml) | mediawiki-action-api | 1 |
| [Wiktionary MediaWiki Action API — OpenSearch](capabilities/mediawiki-action-api-opensearch.yaml) | mediawiki-action-api | 1 |
| [Wiktionary MediaWiki Action API — Parse](capabilities/mediawiki-action-api-parse.yaml) | mediawiki-action-api | 1 |
| [Wiktionary MediaWiki Action API — Query](capabilities/mediawiki-action-api-query.yaml) | mediawiki-action-api | 4 |
| [Wiktionary Wikimedia REST API — Definition](capabilities/rest-api-definition.yaml) | rest-api | 1 |
| [Wiktionary Wikimedia REST API — Page Content](capabilities/rest-api-page-content.yaml) | rest-api | 4 |
| [Wiktionary Wikimedia REST API — Transform](capabilities/rest-api-transform.yaml) | rest-api | 3 |

## Vocabulary

- [Wiktionary Vocabulary](vocabulary/wiktionary-vocabulary.yml) — Unified taxonomy mapping 9 resources, 8 actions, 11 workflows, and 8 personas across operational (OpenAPI) and capability (Naftiko) dimensions

## Rules

- [wiktionary-spectral-rules.yml](rules/wiktionary-spectral-rules.yml) — 41 rules enforcing Wiktionary / Wikimedia API conventions

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
