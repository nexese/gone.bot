# Epsilon

- ID: `epsilon`
- Category: marketing
- Jurisdictions: international request form; rights vary by residence, with opt-out choices broadly offered to U.S. consumers acting for themselves
- Review status: reviewed guidance
- Last reviewed: 2026-08-14

## Official sources

- Consumer request form: <https://legal.epsilon.com/dsr>
- Consumer information and preference center: <https://legal.epsilon.com/us/consumer-information>
- U.S. products privacy policy: <https://legal.epsilon.com/us/NA-products-privacy-policy>

## Supported goals

- `delete` — when offered by the live form and applicable to the user's residence.
- `opt-out` — use the exact live choice, which may distinguish sale or sharing, targeted advertising, profiling or automated decision-making, and sensitive-information use.
- `appeal` — use only when the user has an actual denial and the current form offers an appeal for their residence.

## Channels and required capabilities

- Channel: browser form or the official telephone alternative
- Harness capabilities: browser and filesystem; email or phone may be required for verification or response
- Destination: <https://legal.epsilon.com/dsr>

## Minimum known fields

- Country — routes the reviewed form
- Request goal — identifies the privacy choice requested
- Identity and contact values required by the routed form — entered directly by the user

## Procedure

1. Ask the user for the intended goal and country or residence only to route the official form.
2. Open Epsilon's request page and confirm the current choices and fields.
3. Explain the selected choice literally; do not collapse sale/sharing opt-out, targeted-advertising opt-out, profiling opt-out, and deletion into one outcome.
4. The user completes identity questions, attestations, and submission.
5. Record the chosen request, date, broad status, and non-secret reference separately from any later response.

## Manual checkpoints

- CAPTCHA: unknown; manual if shown
- MFA or OTP: unknown; manual if shown
- Login: not observed at the entry step
- Identity documents: not expected from the reviewed consumer guidance; stop if requested
- Other: verification questions and appeals are always user-controlled

## Evidence and status interpretation

Submission proves only that a request was sent. An opt-out may create or retain a suppression marker rather than erase all data. Deletion, appeal, and each opt-out category must remain separate statuses.

## Limitations

- Available rights, exceptions, verification, and appeal processes depend on current law and residence.
- Epsilon's choices affect Epsilon-controlled processing and do not promise removal from unrelated marketers.
- Do not encode response deadlines; follow the current notice and the broker's actual messages.
