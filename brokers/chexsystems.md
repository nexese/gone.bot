# ChexSystems

- ID: `chexsystems`
- Category: specialty reporting — checking and bank accounts
- Jurisdictions: United States
- Review status: reviewed freeze guidance
- Last reviewed: 2026-08-17

## Official sources

- Security freeze: <https://www.chexsystems.com/security-freeze>
- Freeze portal: <https://www.chexsystems.com/security-freeze/place-freeze>

## Supported goals

- `freeze` — restrict release of the user's ChexSystems consumer report when deletion or ordinary opt-out is unavailable. This does not erase the file.
- `block` — use only when the official portal offers a block for the user's stated circumstances; do not infer eligibility.

## Channels and required capabilities

- Channel: browser portal, telephone, or postal mail
- Harness capabilities: browser and filesystem; the user handles account authentication and sensitive fields
- Destination: start at the official security-freeze page

## Minimum known fields

The live portal determines the fields. Identity data, any freeze PIN, and supporting documents remain user-handled and are never recorded in GoneBot progress.

## Procedure

1. Explain that the freeze restricts the ChexSystems report and may affect opening a bank or credit-union account.
2. Open the official freeze page and review the current channel and required fields.
3. The user completes authentication, sensitive fields, and final submission.
4. Record only the company, date, scope, status, and a non-secret confirmation reference.

## Manual checkpoints

- Login, PIN, knowledge questions, identity documents, CAPTCHA, and final submission are user-handled.

## Evidence and status interpretation

A portal confirmation establishes only that ChexSystems reports the freeze active. It is not deletion and does not establish a freeze at another consumer reporting company.

## Limitations

- Access exceptions may apply. Review the current official notice.
- The user may need a temporary lift before legitimate deposit-account applications.
- Store recovery information outside GoneBot progress in a secure location chosen by the user.
