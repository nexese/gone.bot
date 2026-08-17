# Clarity Services

- ID: `clarity-services`
- Category: specialty reporting — alternative financial services
- Jurisdictions: United States
- Review status: reviewed freeze guidance
- Last reviewed: 2026-08-17

## Official sources

- Consumer portal: <https://consumers.clarityservices.com/>
- Security freeze information: <https://www.clarityservices.com/support/security-freeze/>
- CFPB company list: <https://www.consumerfinance.gov/consumer-tools/credit-reports-and-scores/consumer-reporting-companies/companies-list/>

## Supported goals

- `freeze` — restrict release of the Clarity Services consumer report when deletion is unavailable. It does not erase the file or freeze Experian's nationwide credit report.

## Channels and required capabilities

- Channel: official browser portal, telephone, or postal alternative
- Harness capabilities: browser and filesystem; user handles sensitive entry and verification
- Destination: Clarity Services consumer portal

## Minimum known fields

Use only live official fields. Keep identifiers, documents, authentication answers, and recovery information out of chat and progress.

## Procedure

1. Explain the alternative-financial-services scope and that Experian ownership does not make this the same as an Experian credit freeze.
2. Warn about possible effects on legitimate lending or telecom applications.
3. Preview and approve the Clarity-specific request.
4. The user submits; record minimal confirmation and lift guidance.

## Manual checkpoints

- Login, CAPTCHA, MFA, sensitive values, documents, and final submission are user-handled.

## Evidence and status interpretation

A Clarity confirmation is not deletion and does not establish any other Experian freeze.

## Limitations

- Review the live notice for covered products, access exceptions, and current procedures.
