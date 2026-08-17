# FactorTrust

- ID: `factortrust`
- Category: specialty reporting — nonprime lending
- Jurisdictions: United States
- Review status: reviewed freeze guidance
- Last reviewed: 2026-08-17

## Official sources

- Consumer freeze portal: <https://lpconsumerportal.transunion.com/Consumer/CreditFreeze/Landing.aspx>
- CFPB company list: <https://www.consumerfinance.gov/consumer-tools/credit-reports-and-scores/consumer-reporting-companies/companies-list/>

## Supported goals

- `freeze` — restrict release of the FactorTrust consumer report when deletion is unavailable. It does not erase the file or freeze TransUnion's nationwide credit report.

## Channels and required capabilities

- Channel: TransUnion-hosted FactorTrust browser portal or current official alternative
- Harness capabilities: browser and filesystem; user handles sensitive fields and verification
- Destination: official FactorTrust consumer freeze portal

## Minimum known fields

The live portal controls. Do not retain identifiers, documents, authentication answers, or recovery information.

## Procedure

1. Explain FactorTrust's nonprime-report scope and separate relationship to TransUnion.
2. Warn that lenders may be unable to access the report during legitimate applications.
3. Preview and approve the FactorTrust-specific action.
4. The user completes verification and submission; record minimal confirmation.

## Manual checkpoints

- CAPTCHA, authentication, sensitive values, identity documents, and final submission are user-handled.

## Evidence and status interpretation

A FactorTrust confirmation is not deletion and does not freeze TransUnion or another specialty report.

## Limitations

- Access exceptions and product coverage are controlled by the current official notice.
