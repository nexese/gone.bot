# Acxiom

- ID: `acxiom`
- Category: marketing
- Jurisdictions: international entry point; available choices depend on country and residence
- Review status: reviewed entry-point guidance
- Last reviewed: 2026-08-14

## Official sources

- Acxiom privacy center: <https://www.acxiom.com/privacy/>
- Consumer rights portal: <https://privacyportal.onetrust.com/webform/342ca6ac-4177-4827-b61e-19070296cbd3/6896cf25-6953-4500-9c69-5a8fb6f6f932>

## Supported goals

- `delete` and `opt-out` — only as presented by the live portal for the user's country and residence.
- `opt-out` may include a distinct request to limit sensitive-personal-information use when the portal offers it.

## Channels and required capabilities

- Channel: browser form hosted on Acxiom's configured OneTrust privacy portal
- Harness capabilities: browser and filesystem; email may be required for verification or response
- Destination: use the consumer portal linked from Acxiom's current privacy center

## Minimum known fields

- Country of residence — required by the reviewed entry page to route the request
- Removal goal — selects deletion, opt-out, or sensitive-information limitation when offered
- Other identifying fields — determined by the live routed form and entered by the user

## Procedure

1. Start at Acxiom's privacy center and follow its consumer-rights link rather than trusting a copied portal address alone.
2. Confirm the expected Acxiom-branded OneTrust portal and let the user select their country.
3. Select only the request goal the user stated and review the routed form before entering values.
4. The user completes identity verification, attestations, and final submission.
5. Record the request type, date, broad status, and non-secret reference; keep later responses distinct.

## Manual checkpoints

- CAPTCHA: unknown; manual if shown
- MFA or OTP: unknown; manual if shown
- Login: not observed at the country-routing step
- Identity documents: possible in a routed verification flow; always user-handled and never stored
- Other: a redirect to `privacyportal.onetrust.com` is expected only when reached from Acxiom's official privacy center

## Evidence and status interpretation

Portal submission is evidence that a request was sent. It does not establish that Acxiom matched a record or completed the requested action. Record denials, partial outcomes, and completions exactly as reported.

## Limitations

- Rights, verification, exceptions, and available goals vary by country and residence.
- An opt-out is not necessarily deletion, and limiting one use does not imply all processing stopped.
- Re-enter through Acxiom's privacy center if the third-party portal URL or branding changes.
