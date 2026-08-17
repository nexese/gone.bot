# PeopleConnect Suppression Center

- ID: `peopleconnect`
- Category: people search
- Jurisdictions: suppression tool offered for personal use; privacy rights vary by residence
- Review status: reviewed guidance
- Last reviewed: 2026-08-14

## Official sources

- Suppression Center: <https://suppression.peopleconnect.us/>
- Privacy Center: <https://suppression.peopleconnect.us/privacy-center>
- Terms of Use: <https://peopleconnect.us/terms-of-use/>

## Supported goals

- `opt-out` — manage display of a background report returned by name search on covered PeopleConnect people-search sites.

Deleting Suppression Center user data is not a supported removal action because it can also delete saved suppressions and make the public report searchable again.

## Channels and required capabilities

- Channel: browser flow with email authentication
- Harness capabilities: browser, email, and filesystem
- Destination: <https://suppression.peopleconnect.us/>

## Minimum known fields

- User-controlled email address — starts authentication and maintains the suppression
- Identifying information requested by the live tool — used to locate the user's public-data report; enter directly in the official flow

## Procedure

1. Explain that the tool covers name-search background reports on the PeopleConnect sites identified by its current terms, including TruthFinder, Instant Checkmate, Intelius, and US Search.
2. Warn that suppression and deletion of Suppression Center user data have opposite effects on the saved suppression.
3. Open the official Suppression Center and let the user authenticate by email.
4. The user selects their own report, chooses its display setting, and submits it directly.
5. Record the covered service, date, display choice, and non-secret acknowledgment; do not store authentication details.

## Manual checkpoints

- CAPTCHA: manual if shown
- MFA or OTP: email authentication is manual
- Login: email-authenticated session required
- Identity documents: not observed; stop if requested
- Other: this profile supports only the user's personal request, not agent or commercial use

## Evidence and status interpretation

The saved display choice is evidence of a suppression setting, not deletion. A missing name-search report supports only the covered name-search context checked. Keep the Suppression Center account or user-data record if needed to maintain the suppression.

## Limitations

- The current terms describe coverage for TruthFinder, Instant Checkmate, Intelius, US Search, and additional affiliated sites, but the live terms control the exact list.
- Suppression does not cover user-account data, Classmates, third-party sources, every phone/address/email search, or legally required public displays such as certain offender lists.
- Public-record discrepancies can produce another result that needs separate review.
