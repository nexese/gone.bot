# Teletrack

- ID: `teletrack`
- Category: specialty reporting — subprime lending and services
- Jurisdictions: United States
- Review status: reviewed freeze guidance
- Last reviewed: 2026-08-17

## Official sources

- Consumer portal: <https://consumers.teletrack.com/>
- CFPB 2025 company list: <https://files.consumerfinance.gov/f/documents/cfpb_consumer-reporting-companies_list_2025.pdf>

## Supported goals

- `freeze` — restrict release of the Teletrack consumer report when deletion is unavailable. This does not erase the file or freeze Equifax.

## Channels and required capabilities

- Channel: official consumer portal, telephone, or postal alternative shown by the live site
- Harness capabilities: browser and filesystem; user handles sensitive fields and verification
- Destination: Teletrack consumer portal

## Minimum known fields

The live official channel controls. Keep identifiers, documents, authentication answers, and recovery information out of chat and progress.

## Procedure

1. Explain Teletrack's specialty-report scope and possible effect on legitimate subprime credit, rent-to-own, telecom, or related applications.
2. Verify the live freeze process.
3. Preview and approve the Teletrack-specific action.
4. The user completes sensitive and final steps; record minimal confirmation.

## Manual checkpoints

- Authentication, CAPTCHA, sensitive identifiers, documents, and final submission are user-handled.

## Evidence and status interpretation

A Teletrack confirmation is not deletion and does not establish an Equifax or other-company freeze.

## Limitations

- Equifax ownership does not merge the freeze controls.
- Review the current official notice for exceptions and lift/removal instructions.
