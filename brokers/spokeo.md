# Spokeo

- ID: `spokeo`
- Category: people search
- Jurisdictions: public listing opt-out appears generally available; statutory removal choices vary by residence
- Review status: reviewed guidance
- Last reviewed: 2026-08-25

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

- Spokeo profile URL — identifies the listing to suppress. A user may share a privacy-controls URL with the agent in the current conversation so the agent can derive the canonical form; do not retain either URL or its token in the progress file.
- Email address — receives the confirmation step

## Procedure

1. Ask the user to confirm that the listing is theirs; do not infer identity from a name match.
2. Give the user both official links and explain their order without waiting for a follow-up question:
   - **Find the listing:** <https://www.spokeo.com/privacy/control>. Privacy Controls may show the user's record at a share-style URL that the opt-out form will not accept.
   - **Submit the suppression request:** <https://www.spokeo.com/optout>. This form needs the canonical profile URL.
3. The user may paste their share-style Privacy Controls URL into the current conversation. Treat it as private session data; use it only to prepare this action, and never copy it, its token, or the derived profile URL into the progress file or repository.
4. When the shared address has a `share_token` query parameter and a final path segment beginning with `t` followed by a long numeric record suffix, derive the canonical profile URL by removing the query string and that final `t...` segment, while preserving the preceding name, state, and city path. For example: `https://www.spokeo.com/First-Last/State/City/t123456789?share_token=example` becomes `https://www.spokeo.com/First-Last/State/City`.
5. Give the derived URL to the user to paste into the official opt-out page. If the form rejects it, do not guess at other URL edits; have the user find or copy the canonical public profile URL through Spokeo's own public search instead.
6. Stop before submission and show the exact destination, disclosed fields, request text, limitations, and proposed progress update.
7. The user completes any CAPTCHA and confirms the email message.
8. Record the acknowledgment separately from any later public-listing recheck. Record only a minimal status, not the profile or confirmation link.

## Manual checkpoints

- CAPTCHA: likely; always manual
- MFA or OTP: email confirmation is manual
- Login: not known to be required for public listing opt-out
- Identity documents: not expected for the public listing flow; stop if requested
- Browser safety controls: some agent browsers may block Spokeo's official pages. In that case, give the user the official opt-out URL for a fully manual completion, do not claim the page was opened or a request was submitted, and ask only for a non-sensitive outcome to update the progress record.
- Other: repeat only for additional listings the user individually confirms

## Evidence and status interpretation

An email confirmation or on-screen acknowledgment is evidence of a submitted suppression request, not proof of deletion from all Spokeo systems. A later missing public listing is evidence only that the checked URL is no longer public.

## Limitations

- The official opt-out page was not readable by the documentation tool during this review; the live form is authoritative.
- Privacy Controls can produce a share-style record URL that the opt-out form does not accept. The narrowly described canonical-URL conversion above is an observed manual workaround, not a promise that it will apply to every listing or future site design.
- Spokeo's statutory privacy controls and eligibility vary. Never guess which right applies.
- Public records or a new listing can cause information to reappear.
