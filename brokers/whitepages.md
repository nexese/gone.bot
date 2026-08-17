# Whitepages

- ID: `whitepages`
- Category: people search
- Jurisdictions: public listing suppression appears generally available; statutory privacy rights vary by residence
- Review status: limited guidance; live form not readable during review
- Last reviewed: 2026-08-14

## Official sources

- Public listing suppression: <https://www.whitepages.com/suppression-requests>
- Privacy information: <https://www.whitepages.com/privacy-policy>

## Supported goals

- `opt-out` — request suppression of a specific public Whitepages listing.
- `delete` — use only a deletion choice actually offered by the current privacy flow for the user's residence; do not describe listing suppression as system-wide deletion.

## Channels and required capabilities

- Channel: browser form with user-completed verification
- Harness capabilities: browser and filesystem; phone or email may be needed by the live flow
- Destination: <https://www.whitepages.com/suppression-requests>

## Minimum known fields

The official pages blocked documentation access during review. Do not pre-collect fields from third-party instructions. The user should identify their exact listing and enter only the information the live official flow requires.

## Procedure

1. Ask the user to select and confirm their own public listing; do not choose a record from name similarity alone.
2. Open the official suppression page and confirm the destination remains on `whitepages.com` or a destination linked from its current privacy page.
3. Hand control to the user for all record selection, verification, and submission steps.
4. Record the submitted listing URL, date, broad status, and non-secret acknowledgment the user chooses to retain.
5. Treat any later check as evidence about that listing only.

## Manual checkpoints

- CAPTCHA: unknown; always manual if shown
- MFA or OTP: unknown; always manual if shown
- Login: unknown
- Identity documents: not reviewed; stop if requested and let the user assess the official flow
- Other: separate public suppression from any jurisdiction-specific removal request

## Evidence and status interpretation

An on-screen or message acknowledgment shows only that a request was submitted or received. A missing public listing supports suppression of that listing; it does not prove deletion from Whitepages systems, public records, cached results, or third parties.

## Limitations

- The official pages returned access controls to the documentation tools during this review, so their live fields and verification method remain unreviewed.
- Repeat only for additional listings the user individually confirms.
- Stop if the destination, requested data, or stated effect differs materially from this profile.
