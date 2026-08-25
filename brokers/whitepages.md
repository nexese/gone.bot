# Whitepages

- ID: `whitepages`
- Category: people search
- Jurisdictions: public listing suppression appears generally available; statutory privacy rights vary by residence
- Review status: limited guidance; live form not readable during review
- Last reviewed: 2026-08-25

## Official sources

- Find a listing: <https://www.whitepages.com/>
- Public listing suppression: <https://www.whitepages.com/suppression-requests>
- Privacy information: <https://www.whitepages.com/privacy-policy>

## Supported goals

- `opt-out` — request suppression of a specific public Whitepages listing.
- `delete` — use only a deletion choice actually offered by the current privacy flow for the user's residence; do not describe listing suppression as system-wide deletion.

## Channels and required capabilities

- Channel: browser form plus user-completed phone-call verification
- Harness capabilities: browser, filesystem, and a phone the user can answer; email may also be needed by the live flow
- Destination: <https://www.whitepages.com/suppression-requests>

## Minimum known fields

The official pages blocked documentation access during review. Do not pre-collect fields from third-party instructions. The user should identify their exact listing and enter only the information the live official flow requires. The suppression form requires the Whitepages URL for the selected record; a user may share it in the current conversation for assistance, but it must not be retained in the progress file.

## Procedure

1. Ask the user to select and confirm their own public listing; do not choose a record from name similarity alone.
2. Give the user both official links and explain their order without waiting for a follow-up question:
   - **Find the listing:** <https://www.whitepages.com/>. The user searches and opens their own result.
   - **Submit the suppression request:** <https://www.whitepages.com/suppression-requests>. The user pastes the selected record's Whitepages URL into this form.
3. Use the canonical profile link from the selected search result, whose observed shape is `https://www.whitepages.com/name/Name/City-State/RecordId`. Paste that profile link into the suppression form unchanged.
4. Opening a search result may instead navigate to a Whitepages checkout or summary page. That checkout URL is not the profile link to submit. Have the user return to the search results and copy the selected result's profile-link address; do not attempt to derive it from the checkout URL.
5. The user may share a profile link in the current conversation if agent assistance is useful. Treat it as private session data, and do not copy it into the progress file or repository.
6. If the user has multiple listings, have them individually confirm each listing. Prepare and submit a separate suppression request for each confirmed profile link; do not infer that suppression of one listing covers the others.
7. Before each submission, show the exact destination, disclosed fields, request text, limitations, and proposed progress update. Hand control to the user for all record selection, verification, and submission steps.
8. The observed live opt-out flow places a phone call with a confirmation code. The user must answer the call and enter the code themselves to complete the request. Do not ask them to share the code, and do not record it. Stop and explain the changed flow if phone verification is not offered or another verification method appears.
9. Record only the date, broad status, and non-secret acknowledgment the user chooses to retain. Treat any later check as evidence about that listing only.

## Manual checkpoints

- CAPTCHA: unknown; always manual if shown
- MFA or OTP: phone-call confirmation code is required in the observed opt-out flow; always manual. Do not request, receive, or store the code.
- Login: unknown
- Identity documents: not reviewed; stop if requested and let the user assess the official flow
- Browser safety controls: agent browsers may block Whitepages' official pages. In that case, give the user the two official links above for a fully manual completion, do not claim that a page was opened or request was submitted, and ask only for a non-sensitive outcome to update the progress record.
- Other: separate public suppression from any jurisdiction-specific removal request

## Evidence and status interpretation

An on-screen acknowledgment before the phone confirmation is evidence only of an incomplete or pending request. A completion acknowledgment after the user enters the phone-call code is evidence that the opt-out was submitted or received. A missing public listing supports suppression of that listing; it does not prove deletion from Whitepages systems, public records, cached results, or third parties.

## Limitations

- The official pages returned access controls to the documentation tools during this review, so their live fields and verification method remain unreviewed.
- A selected result may open a checkout or summary URL. The observed suppression input is instead the canonical `/name/.../<record-id>` profile link from the search results. This is not a promise that every current or future Whitepages URL will be accepted.
- The observed opt-out flow required a phone call and confirmation code to complete each request; its precise prompt or timing may change.
- Repeat separately for each additional listing the user individually confirms.
- Stop if the destination, requested data, or stated effect differs materially from this profile.
