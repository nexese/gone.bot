# BeenVerified

- ID: `beenverified`
- Category: people search
- Jurisdictions: public listing opt-out appears generally available; statutory privacy rights vary by residence
- Review status: limited guidance; live form not readable during review
- Last reviewed: 2026-08-14

## Official sources

- Public listing opt-out: <https://www.beenverified.com/svc/optout/search/optouts>
- Privacy information: <https://www.beenverified.com/faq/privacy/>

## Supported goals

- `opt-out` — request that a user-confirmed public result be excluded from BeenVerified's people-search results.
- `delete` — use only when the live official privacy flow expressly offers deletion for the user's residence; do not infer it from a public-result opt-out.

## Channels and required capabilities

- Channel: browser form with user-completed verification
- Harness capabilities: browser and filesystem; email may be needed by the live flow
- Destination: <https://www.beenverified.com/svc/optout/search/optouts>

## Minimum known fields

The official opt-out page blocked documentation access during review. Do not pre-collect fields from third-party guides. The user should select their own result and provide only values required by the current official form.

## Procedure

1. Open the official opt-out page and let the user search for and select their own result.
2. Do not choose among people with similar names or expose unrelated search results in the progress file.
3. The user enters any contact or verification values directly and completes submission.
4. Record only the result identifier or URL the user approves, date, broad status, and a non-secret acknowledgment.
5. Recheck only if the user requests monitoring and keep the outcome scoped to BeenVerified.

## Manual checkpoints

- CAPTCHA: unknown; always manual if shown
- MFA or OTP: unknown; always manual if shown
- Login: unknown
- Identity documents: not reviewed; stop if requested
- Other: result selection is always user-controlled

## Evidence and status interpretation

A submitted request or confirmation message is not proof that every BeenVerified record has been removed. A later absent result is evidence only for the query and result checked, not deletion from source records, affiliates, caches, or other services.

## Limitations

- The official opt-out endpoint returned access controls to the documentation tools during this review, so the live fields and verification method remain authoritative.
- Brand coverage and affiliate effects were not verified and must not be promised.
- Stop if the live flow redirects unexpectedly or makes a materially different claim.
