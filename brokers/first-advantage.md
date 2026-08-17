# First Advantage

- ID: `first-advantage`
- Category: specialty reporting — employment background screening
- Jurisdictions: United States
- Review status: reviewed freeze guidance
- Last reviewed: 2026-08-17

## Official sources

- Candidate consumer help and freeze form: <https://fadv.com/candidates/>
- CFPB 2025 company list: <https://files.consumerfinance.gov/f/documents/cfpb_consumer-reporting-companies_list_2025.pdf>

## Supported goals

- `freeze` — restrict release of First Advantage consumer files when deletion is unavailable. This does not erase prior reports or public/source records.

## Channels and required capabilities

- Channel: official browser form, telephone, email, or postal mail
- Harness capabilities: browser, email, and filesystem; user handles CAPTCHA and sensitive fields
- Destination: First Advantage candidate page, under “How Can I Place A Freeze On My Data?”

## Minimum known fields

The reviewed form asks for name, date of birth, email, phone, and the organization that requested the background check. Recheck the live form and let the user enter sensitive values directly.

## Procedure

1. Explain that a freeze may delay or prevent a legitimate employer or other requester from completing a background screen.
2. Confirm there is no imminent screening the user wants to allow.
3. Preview the exact channel, fields, and consequence; obtain approval.
4. The user completes CAPTCHA, verification, and submission.

## Manual checkpoints

- CAPTCHA, date of birth and other sensitive values, identity documents, and final submission are user-handled.

## Evidence and status interpretation

A submitted form is not an active freeze until confirmed. A freeze is not deletion and does not remove information at source providers.

## Limitations

- First Advantage has multiple products. Confirm the live response identifies the files covered.
- Separate tenant-screening controls may be required for Resident Solutions.
