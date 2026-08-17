# Spokeo

- ID: `spokeo`
- Category: people search
- Jurisdictions: public listing opt-out appears generally available; statutory removal choices vary by residence
- Review status: reviewed guidance
- Last reviewed: 2026-08-14

## Official sources

- Public listing opt-out: <https://www.spokeo.com/optout>
- Privacy controls: <https://www.spokeo.com/privacy/control>
- California registration record: <https://www.oag.ca.gov/data-broker/registration/186310>

## Supported goals

- `opt-out` — request suppression of a specific public Spokeo listing.
- `delete` — use only a deletion option actually offered by the live privacy-control flow for the user's jurisdiction; do not treat listing suppression as database deletion.

## Channels and required capabilities

- Channel: browser form plus email confirmation
- Harness capabilities: browser, email, and filesystem
- Destination: <https://www.spokeo.com/optout>

## Minimum known fields

- Spokeo profile URL — identifies the listing to suppress
- Email address — receives the confirmation step

## Procedure

1. Ask the user to confirm that the listing is theirs; do not infer identity from a name match.
2. Capture the exact public profile URL selected by the user.
3. Open the official opt-out page and prepare the profile URL and user-approved email address.
4. Stop before submission and show the exact values and destination.
5. The user completes any CAPTCHA and confirms the email message.
6. Record the acknowledgment separately from any later public-listing recheck.

## Manual checkpoints

- CAPTCHA: likely; always manual
- MFA or OTP: email confirmation is manual
- Login: not known to be required for public listing opt-out
- Identity documents: not expected for the public listing flow; stop if requested
- Other: repeat only for additional listings the user individually confirms

## Evidence and status interpretation

An email confirmation or on-screen acknowledgment is evidence of a submitted suppression request, not proof of deletion from all Spokeo systems. A later missing public listing is evidence only that the checked URL is no longer public.

## Limitations

- The official opt-out page was not readable by the documentation tool during this review; the live form is authoritative.
- Spokeo's statutory privacy controls and eligibility vary. Never guess which right applies.
- Public records or a new listing can cause information to reappear.
