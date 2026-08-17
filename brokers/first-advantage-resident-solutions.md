# First Advantage Resident Solutions

- ID: `first-advantage-resident-solutions`
- Category: specialty reporting — tenant screening
- Jurisdictions: United States
- Review status: reviewed manual freeze guidance
- Last reviewed: 2026-08-17

## Official sources

- First Advantage candidate consumer support: <https://fadv.com/candidates/>
- CFPB 2025 company list: <https://files.consumerfinance.gov/f/documents/cfpb_consumer-reporting-companies_list_2025.pdf>

## Supported goals

- `freeze` — the CFPB listing says First Advantage Resident Solutions accepts freeze requests by telephone or email. This restricts release rather than erasing tenant-screening data.

## Channels and required capabilities

- Channel: current official telephone or `consumer.documents@fadv.com` email route
- Harness capabilities: email and filesystem; telephone and sensitive identity handling are manual
- Destination: verify the current address and product name through First Advantage's candidate consumer support before use

## Minimum known fields

Ask only for fields required by the current official channel. The user supplies DOB, identifiers, documents, and signatures directly when required.

## Procedure

1. Explain that a freeze may delay or prevent a legitimate rental application.
2. Confirm no imminent tenant screen needs access.
3. Verify the current destination and preview exact text and disclosed fields.
4. Obtain approval; the user completes sensitive or telephone steps.

## Manual checkpoints

- Telephone, sensitive values, documents, signature, verification, and final submission are user-handled.

## Evidence and status interpretation

A sent email is not an active freeze until confirmed. The freeze is not deletion and may not cover other First Advantage products.

## Limitations

- Product naming and contact routes can change. Recheck before use.
- The user may need to lift the freeze before a rental application.
