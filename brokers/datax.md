# DataX

- ID: `datax`
- Category: specialty reporting — subprime lending
- Jurisdictions: United States
- Review status: reviewed manual freeze guidance
- Last reviewed: 2026-08-17

## Official sources

- DataX consumer freeze: <https://consumers.dataxltd.com/consumerCreditFreeze>
- DataX prescreen opt-out: <https://consumers.dataxltd.com/consumerOptOut>
- CFPB 2025 company list: <https://files.consumerfinance.gov/f/documents/cfpb_consumer-reporting-companies_list_2025.pdf>

## Supported goals

- `opt-out` — remove a matched file from DataX prescreen lists for five years by phone or permanently by postal form.
- `freeze` — DataX accepts online or postal requests to restrict access to its consumer report. A freeze does not erase the file or freeze Equifax.

## Channels and required capabilities

- Channel: official browser freeze portal or postal mail; prescreen opt-out uses telephone or postal mail
- Harness capabilities: browser and filesystem; printing, calling, and mailing are manual
- Destination: start at the applicable DataX consumer page

## Minimum known fields

Use only the current official form or instructions. The user supplies identifiers, documents, and signature directly; do not place their values in chat or progress.

## Procedure

1. Explain DataX's subprime-report scope and its separation from Equifax.
2. Warn that a freeze may affect legitimate specialty-credit applications.
3. Verify the current online or postal requirements, preview the action, and obtain approval.
4. The user completes sensitive online fields or prints, signs, supplies sensitive material, and mails it.

## Manual checkpoints

- Printing, signature, identity documents, sensitive identifiers, postage, and mailing are user-handled.

## Evidence and status interpretation

Mailing evidence shows only that the request was sent. Record a freeze only after DataX confirms it; this is not deletion.

## Limitations

- Online and postal requirements can change; recheck before disclosure.
- Equifax ownership does not make this equivalent to an Equifax credit freeze.
