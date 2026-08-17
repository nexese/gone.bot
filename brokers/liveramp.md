# LiveRamp

- ID: `liveramp`
- Category: advertising
- Jurisdictions: United States opt-out; deletion depends on residence
- Review status: reviewed guidance
- Last reviewed: 2026-08-14

## Official sources

- Privacy choices: <https://liveramp.com/privacy/my-privacy-choices/>
- Privacy policy: <https://liveramp.com/privacy/service-privacy-policy/>

## Supported goals

- `opt-out` — LiveRamp describes an opt-out choice available across the United States, with separate device- or browser-specific choices also offered.
- `delete` — use only when the live page offers deletion for the user's stated residence.

## Channels and required capabilities

- Channel: browser form, currently routed through a third-party removal request portal
- Harness capabilities: browser, email, and filesystem
- Destination: start at <https://liveramp.com/privacy/my-privacy-choices/>

## Minimum known fields

- First and last name — used for a comprehensive request
- Email address — used for a comprehensive request and responses
- Residence — determines which choices the live flow offers
- Removal goal — opt-out or deletion; keep device-level and comprehensive choices distinct

## Procedure

1. Ask the user for their goal and residence; do not infer legal eligibility.
2. Open LiveRamp's official privacy-choices page and follow only its current official link.
3. Keep device/browser opt-out separate from a comprehensive request.
4. Show the exact request, destination domain, and values before submission.
5. The user completes verification and final submission.
6. Record the portal acknowledgment and later outcome separately.

## Manual checkpoints

- CAPTCHA: unknown; handle manually if shown
- MFA or OTP: possible email verification; always manual
- Login: the linked request portal determines this
- Identity documents: possible during verification; never collect or retain them in GoneBot state
- Other: the user must review any transfer to a third-party request portal

## Evidence and status interpretation

An opt-out is not the same as deletion. A device-level choice is not proof of a comprehensive opt-out. A portal acknowledgment is not proof that LiveRamp found the user or completed the requested action.

## Limitations

- Availability of deletion varies by residence and current law.
- LiveRamp's page and linked request provider can change. Stop if the domain, choices, or requested data differ materially.
