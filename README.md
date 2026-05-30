# HaveIBeenPwned (haveibeenpwned)

Have I Been Pwned (HIBP) is Troy Hunt's free breach-notification and credential-exposure
service. The HIBP API v3 lets clients search for email addresses, pastes, stealer-log
entries, and monitored domains across the world's largest aggregated breach corpus. A
separate free k-anonymity password lookup is offered at api.pwnedpasswords.com.

**APIs.yml:** [apis.yml](apis.yml)

## Type
- **x-type:** company
- **x-tier:** 1 (real profile with artifacts)
- **source:** [public-apis/public-apis](https://github.com/public-apis/public-apis) — category: Security

## APIs

### HIBP API v3
Authenticated REST API for searching breaches, pastes, stealer logs, and monitored
domains. Requires a paid `hibp-api-key`. Public read endpoints (`/breaches`,
`/breach/{name}`, `/latestbreach`, `/dataclasses`) are free and unauthenticated.

- **Documentation:** https://haveibeenpwned.com/API/v3
- **Authentication:** https://haveibeenpwned.com/API/Key (`hibp-api-key` header)
- **OpenAPI:** [openapi/hibp-openapi.yml](openapi/hibp-openapi.yml)

### Pwned Passwords
Free, unauthenticated k-anonymity API for checking whether a password's SHA-1 (or NTLM)
hash appears in the HIBP credential corpus.

- **Documentation:** https://haveibeenpwned.com/API/v3#PwnedPasswords
- **OpenAPI:** [openapi/pwned-passwords-openapi.yml](openapi/pwned-passwords-openapi.yml)

## Artifacts

| Type | Count | Path |
|---|---|---|
| OpenAPI specs | 2 | [`openapi/`](openapi/) |
| JSON Schema | 6 | [`json-schema/`](json-schema/) |
| JSON Structure | 3 | [`json-structure/`](json-structure/) |
| JSON-LD context | 1 | [`json-ld/`](json-ld/) |
| Examples | 15 | [`examples/`](examples/) |
| Spectral rules | 1 | [`rules/`](rules/) |
| Naftiko capabilities | 4 (1 shared + 3 workflows) | [`capabilities/`](capabilities/) |
| Vocabulary | 1 | [`vocabulary/`](vocabulary/) |
| Plans / Pricing | 1 | [`plans/`](plans/) |
| Rate Limits | 1 | [`rate-limits/`](rate-limits/) |
| FinOps | 1 | [`finops/`](finops/) |

## Pricing Tiers

| Tier | Price (USD/mo) | RPM | Stealer Logs | K-Anon |
|---|---|---|---|---|
| Pwned 1 | $3.95 | 10 | no | no |
| Pwned 2 | $19.45 | 50 | yes | yes |
| Pwned 3 | $109 | 500 | yes | yes |
| Pwned 4 | $275 | 1,000 | yes | yes |
| Pwned 5 | $995 | 5,000 | yes | yes |
| Pwned Passwords | Free | unlimited | n/a | n/a |

See [plans/haveibeenpwned-plans-pricing.yml](plans/haveibeenpwned-plans-pricing.yml) and
[rate-limits/haveibeenpwned-rate-limits.yml](rate-limits/haveibeenpwned-rate-limits.yml)
for the full breakdown.

## GitHub Organization

[github.com/HaveIBeenPwned](https://github.com/HaveIBeenPwned) hosts the public reference
implementations and tooling:

- [PwnedPasswordsAzureFunction](https://github.com/HaveIBeenPwned/PwnedPasswordsAzureFunction) — k-anonymity password API on Azure Functions
- [PwnedPasswordsCloudflareWorker](https://github.com/HaveIBeenPwned/PwnedPasswordsCloudflareWorker) — Cloudflare Worker implementation
- [PwnedPasswordsDownloader](https://github.com/HaveIBeenPwned/PwnedPasswordsDownloader) — CLI to download all password hash ranges
- [EmailAddressExtractor](https://github.com/HaveIBeenPwned/EmailAddressExtractor) — CLI to extract emails from breach files
- [cloudflare-prometheus-exporter](https://github.com/HaveIBeenPwned/cloudflare-prometheus-exporter) — Operational tooling
- [Branding](https://github.com/HaveIBeenPwned/Branding) — Logos and brand assets
- [ux-rebuild](https://github.com/HaveIBeenPwned/ux-rebuild) — UX rebuild collaboration

No first-party MCP server or Claude Code skill is published by HaveIBeenPwned at this time.

## Tags
Security, Breach Notification, Credential Stuffing, Stealer Logs, K-Anonymity, Privacy, Identity

## Timestamps
- **Created:** 2026-05-28
- **Modified:** 2026-05-30

## Maintainers
- **Kin Lane** — kin@apievangelist.com
