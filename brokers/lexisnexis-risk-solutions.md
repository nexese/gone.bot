# LexisNexis Risk Solutions and SageStream

- ID: `lexisnexis-risk-solutions`
- Category: specialty reporting
- Jurisdictions: United States consumer-report freeze; privacy choices vary by residence
- Review status: reviewed guidance
- Last reviewed: 2026-08-17

## Official sources

- Consumer freeze: <https://consumer.risk.lexisnexis.com/freeze>
- Privacy opt-out and suppression: <https://consumer.risk.lexisnexis.com/opt>
- CFPB company entry: <https://www.consumerfinance.gov/consumer-tools/credit-reports-and-scores/consumer-reporting-companies/companies-list/lexis-nexis-risk-solutions/>

## Supported goals

- `delete` or `opt-out` — use only when the privacy portal offers the choice for the user's residence and data.
- `suppress` — limited official suppression may be available for qualifying safety circumstances; do not determine eligibility.
- `freeze` — restrict release of specified LexisNexis Risk Solutions and SageStream consumer reports when removal is unavailable. This does not erase source data or cover unrelated bureaus.

## Channels and required capabilities

- Channel: browser portal or reviewed postal alternative
- Harness capabilities: browser and filesystem; email may be used for responses
- Destination: choose the exact official privacy or freeze page matching the approved goal

## Minimum known fields

Use only the fields in the live official flow. The user enters government identifiers, identity documents, authentication answers, and recovery information directly.

## Procedure

1. Check whether an applicable deletion, opt-out, or suppression choice is available before proposing a freeze.
2. Explain the products covered and possible effects on legitimate credit, insurance, telecom, utility, or other applications.
3. Preview and obtain approval for the exact portal and control.
4. The user completes verification and submission; record only minimal confirmation evidence.

## Manual checkpoints

- Identity verification, sensitive fields, documents, CAPTCHA, login, and final submission are user-handled.

## Evidence and status interpretation

Keep privacy-request and freeze outcomes distinct. A freeze confirmation is not deletion and proves no restriction at an unrelated company.

## Limitations

- Official exceptions may permit some releases.
- Coverage may differ among LexisNexis products; rely on the live notice.
- The user may need to lift the freeze for a legitimate application.
