# LexisNexis C.L.U.E. and Telematics OnDemand

- ID: `lexisnexis-clue`
- Category: specialty reporting — property and auto insurance
- Jurisdictions: United States
- Review status: reviewed freeze guidance
- Last reviewed: 2026-08-17

## Official sources

- Consumer center: <https://consumer.risk.lexisnexis.com/>
- Consumer freeze: <https://consumer.risk.lexisnexis.com/freeze>
- CFPB 2025 company list: <https://files.consumerfinance.gov/f/documents/cfpb_consumer-reporting-companies_list_2025.pdf>

## Supported goals

- `freeze` — restrict release of the applicable C.L.U.E. or Telematics OnDemand consumer report when deletion is unavailable. This does not erase insurance-claims or source data.

## Channels and required capabilities

- Channel: LexisNexis consumer browser portal or current postal/telephone alternative
- Harness capabilities: browser and filesystem; user handles product selection, sensitive fields, and verification
- Destination: start at the official LexisNexis consumer freeze page and choose the applicable U.S. consumer-report product

## Minimum known fields

Use only the current official flow. The user enters identifiers, documents, authentication answers, and recovery information directly.

## Procedure

1. Explain the insurance-report scope and distinguish it from the general LexisNexis/SageStream and nationwide credit-report controls.
2. Warn that a freeze may delay or prevent legitimate property or auto insurance underwriting.
3. Preview the exact product, destination, fields, and consequence; obtain approval.
4. The user completes verification and submission; record minimal confirmation evidence.

## Manual checkpoints

- Product selection, sensitive values, identity documents, CAPTCHA, authentication, and final submission are user-handled.

## Evidence and status interpretation

A confirmation establishes only the product LexisNexis identifies as frozen. It is not deletion and does not prove that another LexisNexis or credit-bureau report is frozen.

## Limitations

- Product names and access exceptions are controlled by the live official page.
- A legitimate insurance application may require a temporary lift.
