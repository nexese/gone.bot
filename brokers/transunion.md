# TransUnion

- ID: `transunion`
- Category: nationwide credit reporting
- Jurisdictions: United States
- Review status: reviewed freeze guidance
- Last reviewed: 2026-08-17

## Official sources

- Security freeze: <https://www.transunion.com/credit-freeze>
- CFPB freeze guidance: <https://www.consumerfinance.gov/ask-cfpb/what-is-a-credit-freeze-or-security-freeze-on-my-credit-report-en-1341/>

## Supported goals

- `freeze` — restrict most new-credit access to the TransUnion credit file when deletion is unavailable. This does not erase the file and has legal access exceptions.

## Channels and required capabilities

- Channel: official browser portal or current telephone/postal alternative
- Harness capabilities: browser and filesystem; the user handles sensitive fields and authentication
- Destination: TransUnion's official freeze page

## Minimum known fields

Use only live official fields. Keep SSN, DOB, documents, passwords, authentication answers, and recovery information out of chat and progress.

## Procedure

1. Explain separate coverage and the possible impact on legitimate applications.
2. Preview the exact official page and requested action.
3. The user authenticates and submits.
4. Record only scope, date, status, non-secret evidence, and the lift path.

## Manual checkpoints

- Account creation, login, CAPTCHA, MFA, identity verification, and final submission are user-handled.

## Evidence and status interpretation

A TransUnion confirmation proves only TransUnion's reported freeze status, not deletion or a freeze at FactorTrust or another specialty company.

## Limitations

- Separate freezes may be needed for FactorTrust and other specialty reports.
- Access exceptions apply; review the current official notice.
