# Equifax

- ID: `equifax`
- Category: nationwide credit reporting
- Jurisdictions: United States
- Review status: reviewed freeze guidance
- Last reviewed: 2026-08-17

## Official sources

- Security freeze: <https://www.equifax.com/personal/credit-report-services/credit-freeze/>
- CFPB freeze guidance: <https://www.consumerfinance.gov/ask-cfpb/what-is-a-credit-freeze-or-security-freeze-on-my-credit-report-en-1341/>

## Supported goals

- `freeze` — restrict most new-credit access to the Equifax credit file when deletion is unavailable. This does not erase the file and has legal access exceptions.

## Channels and required capabilities

- Channel: myEquifax browser portal, telephone, or postal form
- Harness capabilities: browser and filesystem; all sensitive entry and identity verification are user-handled
- Destination: official Equifax freeze page

## Minimum known fields

The live portal or official mail form determines required fields. Never place SSN, DOB, identity documents, authentication answers, or recovery data in chat or progress.

## Procedure

1. Explain that Equifax must be frozen separately from Experian, TransUnion, and specialty reports.
2. Warn that legitimate credit or service applications may be delayed until a lift.
3. Open the official page; the user authenticates and submits.
4. Record minimal confirmation evidence and the official lift path.

## Manual checkpoints

- Account creation, login, CAPTCHA, MFA, identity questions/documents, and submission are user-handled.

## Evidence and status interpretation

An Equifax confirmation proves only Equifax's reported freeze status, not deletion or coverage at another company.

## Limitations

- Some entities retain permitted access. Review current Equifax and CFPB notices.
- The user must manage lifts and recovery information securely outside GoneBot progress.
