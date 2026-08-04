# HaveIBeenPwned (haveibeenpwned)

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

Have I Been Pwned (HIBP) is Troy Hunt's free breach-notification and credential-exposure service. The HIBP API v3 lets clients search for email addresses, pastes, stealer-log entries, and monitored domains across the world's largest aggregated breach corpus. A separate free k-anonymity password lookup is offered at api.pwnedpasswords.com.

**APIs.json:** [https://haveibeenpwned.com/API/v3](https://haveibeenpwned.com/API/v3)

## Tags

- Security
- Breach Notification
- Credential Stuffing
- Stealer Logs
- K-Anonymity
- Privacy
- Identity

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-30

## APIs

### HIBP API v3

Authenticated REST API for searching breaches, pastes, stealer logs, and monitored domains. Requires a paid hibp-api-key. Public read endpoints (/breaches, /breach/{name}, /latestbreach, /dataclasses) are free and unauthenticated.

- **Human URL:** [https://haveibeenpwned.com/API/v3](https://haveibeenpwned.com/API/v3)
- **Base URL:** `https://haveibeenpwned.com/api/v3`

#### Tags

- Security
- Breach
- Stealer Logs

#### Properties

- [Documentation](https://haveibeenpwned.com/API/v3)
- [API Reference](https://haveibeenpwned.com/API/v3)
- [Authentication](https://haveibeenpwned.com/API/Key)
- [OpenAPI](openapi/hibp-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/hibp.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/hibp.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/hibp-breach-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/hibp-paste-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/hibp-subscribed-domain-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/hibp-subscription-status-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/hibp-breached-account-range-entry-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/hibp-breach-structure.json)
- [JSON Structure](json-structure/hibp-paste-structure.json)
- [JSON Structure](json-structure/hibp-subscription-status-structure.json)
- [Example](examples/hibp-get-breaches-for-account-example.json)
- [Example](examples/hibp-get-breaches-by-range-example.json)
- [Example](examples/hibp-list-breaches-example.json)
- [Example](examples/hibp-get-breach-by-name-example.json)
- [Example](examples/hibp-get-latest-breach-example.json)
- [Example](examples/hibp-list-data-classes-example.json)
- [Example](examples/hibp-get-pastes-for-account-example.json)
- [Example](examples/hibp-get-stealer-logs-by-email-example.json)
- [Example](examples/hibp-get-stealer-logs-by-website-domain-example.json)
- [Example](examples/hibp-get-stealer-logs-by-email-domain-example.json)
- [Example](examples/hibp-get-breached-domain-example.json)
- [Example](examples/hibp-list-subscribed-domains-example.json)
- [Example](examples/hibp-get-subscription-status-example.json)
- [Example](examples/hibp-generate-dns-token-example.json)
- [Rate Limits](rate-limits/haveibeenpwned-rate-limits.yml)

### Pwned Passwords

Free, unauthenticated k-anonymity API for checking whether a password's SHA-1 (or NTLM) hash appears in the HIBP credential corpus. Funded by Cloudflare; no API key required.

- **Human URL:** [https://haveibeenpwned.com/API/v3#PwnedPasswords](https://haveibeenpwned.com/API/v3#PwnedPasswords)
- **Base URL:** `https://api.pwnedpasswords.com`

#### Tags

- Security
- Passwords
- K-Anonymity

#### Properties

- [Documentation](https://haveibeenpwned.com/API/v3#PwnedPasswords)
- [OpenAPI](openapi/pwned-passwords-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/pwned-passwords.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/pwned-passwords.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/pwned-passwords-range-result-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Example](examples/pwned-passwords-search-range-example.json)
- [SDK](https://github.com/HaveIBeenPwned/PwnedPasswordsAzureFunction)
- [SDK](https://github.com/HaveIBeenPwned/PwnedPasswordsCloudflareWorker)
- [Tools](https://github.com/HaveIBeenPwned/PwnedPasswordsDownloader)

## Common Properties

- [Website](https://haveibeenpwned.com)
- [Portal](https://haveibeenpwned.com)
- [Sign Up](https://haveibeenpwned.com/API/Key)
- [Pricing](https://haveibeenpwned.com/API/Key)
- [Plans](plans/haveibeenpwned-plans-pricing.yml)
- [Rate Limits](rate-limits/haveibeenpwned-rate-limits.yml)
- [Terms of Service](https://haveibeenpwned.com/API/v3#License)
- [Privacy Policy](https://haveibeenpwned.com/Privacy)
- [Status Page](https://status.haveibeenpwned.com)
- [Blog](https://www.troyhunt.com)
- [GitHub Organization](https://github.com/HaveIBeenPwned)
- [Support](https://haveibeenpwned.com/Contact)
- [F A Q](https://haveibeenpwned.com/FAQs)
- [Public APIs Listing](https://github.com/public-apis/public-apis)
- [Spectral Rules](rules/hibp-rules.yml)
- [JSON-LD](json-ld/haveibeenpwned-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Vocabulary](vocabulary/haveibeenpwned-vocabulary.yml)
- [Tools](https://github.com/HaveIBeenPwned/EmailAddressExtractor)
- [Tools](https://github.com/HaveIBeenPwned/PwnedPasswordsDownloader)
- [Tools](https://github.com/HaveIBeenPwned/cloudflare-prometheus-exporter)
- [Branding](https://github.com/HaveIBeenPwned/Branding)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
