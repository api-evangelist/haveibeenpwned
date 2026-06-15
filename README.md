# HaveIBeenPwned (haveibeenpwned)

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
