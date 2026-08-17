# Data Axle

- ID: `data-axle`
- Category: marketing
- Jurisdictions: United States privacy choices; rights and outcomes may vary by residence
- Review status: reviewed guidance
- Last reviewed: 2026-08-14

## Official sources

- Privacy rights request: <https://www.data-axle.com/privacy-rights-request/>
- Privacy policy: <https://www.data-axle.com/privacy-policy/>

## Supported goals

- `delete` and `opt-out` — only as offered by the current request form and applicable to the user's removal goal.

## Channels and required capabilities

- Channel: browser form
- Harness capabilities: browser and filesystem; email may be needed for responses
- Destination: <https://www.data-axle.com/privacy-rights-request/>

## Minimum known fields

The reviewed form lists these fields. Recheck the live form before collecting anything.

- First and last name — required by the form
- Address — required by the form
- Email — required by the form
- Phone — required by the form
- Privacy choice — required to identify the requested action
- Attestation — the user must make it directly

## Procedure

1. Confirm the request is for the user and select only the privacy choice they state.
2. Open the official form and compare its current fields with this profile.
3. Prepare only the fields required by the live form.
4. Show the user the destination, requested action, and all values before submission.
5. The user completes the attestation, any verification, and final submission.
6. Record the acknowledgment and later response as separate events.

## Manual checkpoints

- CAPTCHA: unknown; handle manually if shown
- MFA or OTP: unknown; handle manually if shown
- Login: not observed on the reviewed request page
- Identity documents: possible during verification; never collect or retain them in GoneBot state
- Other: authorized-agent requests are outside GoneBot's supported scope

## Evidence and status interpretation

Form submission means only that a request was sent. An acknowledgment means Data Axle says it received the request. A response may report completion, denial, partial completion, or a need for verification; preserve those distinctions.

## Limitations

- Rights, exemptions, and response details depend on current law and the information Data Axle can match.
- Never promise that deletion covers public records, third-party copies, or information that must be retained.
