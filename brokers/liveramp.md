# LiveRamp

- ID: `liveramp`
- Category: advertising
- Jurisdictions: country-routed choices, including Canada, the EEA, and the United Kingdom; availability depends on residence and current policy
- Review status: reviewed guidance
- Last reviewed: 2026-08-14

## Reviewed source snapshot

On 2026-08-19, LiveRamp's privacy-center material listed global mobile-identifier and third-party-cookie choices, a Canadian request portal, a United Kingdom portal and privacy contact, and EEA country contacts. This local summary—not a live third-party page—is the planning source for this profile.

## Supported goals

- `opt-out` — LiveRamp presents global mobile-identifier and third-party-cookie choices, plus country-specific rights channels. Keep browser/device choices distinct from a comprehensive request.
- `delete` — use only the deletion or erasure choice presented by the official country route for the user's stated residence.

## Channels and required capabilities

- Channel: browser form or country-specific privacy contact, as routed from LiveRamp's official privacy center
- Harness capabilities: browser, email, and filesystem
- Destination: `liveramp-privacy-center` — resolve only after a user-approved external-navigation preview

## Minimum known fields

- First and last name — used for a comprehensive request
- Email address — used for a comprehensive request and responses
- Country or residence — determines the current official route and available choices; do not infer it
- Removal goal — opt-out or deletion; keep device-level and comprehensive choices distinct

## Procedure

1. Ask the user for their goal and residence; do not infer legal eligibility.
2. After the user approves the external-navigation preview, open only the LiveRamp-branded privacy center and choose the route that matches the user's stated residence.
3. Keep global mobile-identifier or third-party-cookie choices separate from a country-routed comprehensive request.
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

- Availability of deletion and the appropriate country route vary by residence and current policy.
- A country-specific route does not by itself establish legal eligibility. Use the jurisdiction guide and the live form's offered choices.
- Stop if the destination, choices, or requested data differ materially from this reviewed snapshot.
