# Criteo

- ID: `criteo`
- Category: advertising
- Jurisdictions: EEA and United Kingdom rights guidance; browser advertising control is presented globally, while other rights depend on location and current policy
- Review status: reviewed guidance
- Last reviewed: 2026-08-19

## Reviewed source snapshot

On 2026-08-19, Criteo's rights material described an EEA/UK erasure route and a browser-specific service control. The browser control withdrew consent for Criteo services in the current browser, removed Criteo cookies there, and could need repeating after a browser or device change. This local summary—not a live third-party page—is the planning source for this profile.

## Supported goals

- `delete` — Criteo’s rights page directs EEA/UK erasure requests through its current contact form. Use only after the user confirms the relevant location and the live page still offers that route.
- `opt-out` — the browser control withdraws consent to Criteo services for the current browser and deletes Criteo cookies in that browser. It is not a comprehensive deletion request.
- `block` — the same browser control stops Criteo’s consent-based data collection and ads in that browser. Record it as browser-specific and repeat it for other browsers or devices as Criteo instructs.

## Channels and required capabilities

- Channel: browser form or browser-specific Criteo control
- Harness capabilities: browser and filesystem; email may be required for a response
- Destination: `criteo-rights` or `criteo-browser-control` — resolve only after a user-approved external-navigation preview

## Minimum known fields

- Request type — deletion, objection, or current-browser service control
- Country or region — only when the live rights form uses it to route the request
- Browser or device context — only for the browser-specific control
- Other identifiers — live form only; the user enters them directly

## Procedure

1. Confirm whether the user seeks EEA/UK erasure or a browser-specific advertising choice; do not collapse them into one request.
2. After the user approves the external-navigation preview, open only the Criteo-branded destination matching the selected route and compare it with this snapshot.
3. For an erasure request, select only the supported legal or policy choice. For a browser control, explain that it applies to the current browser/device context.
4. Show the exact destination, form selections, disclosed fields, limitations, and local progress entry before submission.
5. The user completes any final verification or browser interaction after explicit approval.

## Manual checkpoints

- CAPTCHA: unknown; manual if shown
- MFA or OTP: unknown; manual if shown
- Login: not observed for the reviewed entry points
- Identity documents: unknown; stop if requested
- Other: Criteo’s rights form requires JavaScript; do not substitute an unverified form or email address if it is unavailable

## Evidence and status interpretation

The browser control evidences a choice in the current browser, not deletion of all Criteo-held information. A submitted rights form proves only that the request was sent. Record later confirmation, denial, retention explanation, or completion as separately observed statuses.

## Limitations

- Criteo says its browser choice is saved in a dedicated cookie and may need to be repeated after clearing browser data, changing devices, or changing the operating system.
- Criteo can continue some processing collected before a browser choice on another stated basis; do not represent the browser choice as global deletion.
- Rights, exceptions, and identity verification depend on location and the live privacy flow.
