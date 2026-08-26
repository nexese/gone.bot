# California DROP

- ID: `california-drop`
- Category: government mechanism
- Jurisdictions: California residents
- Review status: reviewed guidance
- Last reviewed: 2026-08-25

## Official sources

- Program information: <https://privacy.ca.gov/drop/>
- Request portal: <https://consumer.drop.privacy.ca.gov/>

## Supported goals

- `delete` — one request can direct data brokers registered with California to delete covered personal information, subject to the program's scope and legal exceptions.
- `opt-out` — use the choices offered by the live DROP portal; do not promise that every downstream use will stop.

## Channels and required capabilities

- Channel: government browser portal
- Harness capabilities: browser and filesystem
- Destination: <https://consumer.drop.privacy.ca.gov/>

## Minimum known fields

The live portal determines the required fields. California's program information says that a resident verifies identity through California Identity Gateway and chooses what data to provide. Do not pre-collect identity data outside that portal.

## Procedure

1. Confirm that the user is requesting action for themself and says they are a California resident.
2. Open the official request portal and let the user complete identity verification directly.
3. Explain the choices shown by the portal without making an eligibility or legal determination.
4. Stop before final submission and ask the user to review the live request.
5. After the user submits, record only the date, status, and non-secret reference they choose to retain.

## California queue overlap

After a user submits DROP, do not immediately queue separate direct deletion requests to Data Axle, Acxiom, or Epsilon. DROP applies to all current and future active DROP data brokers unless the user narrows their request; wait for the broker-specific DROP status before treating a direct deletion form as necessary. The list and status displayed in the user's DROP account are authoritative for a particular company.

Keep these as separate, non-duplicate cases when the user wants their distinct result:

- Spokeo, Whitepages, BeenVerified, and PeopleConnect — public-listing suppression. DROP does not delete publicly available data, so a public-result suppression can still be useful.
- OptOutPrescreen — firm-offer credit/insurance-list opt-out, not data-broker deletion.

Defer Cotality's direct privacy route until DROP reports a status or the user identifies a separate need. Its property/public or consumer-reporting data can be outside DROP's deletion scope or legally exempt.

## Manual checkpoints

- CAPTCHA: unknown; handle manually if shown
- MFA or OTP: identity verification is manual
- Login: California Identity Gateway may be required
- Identity documents: do not collect; the user handles any request in the official portal
- Other: never attempt to act for a minor, dependent, or another adult

## Evidence and status interpretation

A portal confirmation means only that DROP accepted the request. Broker processing and deletion are later states. Do not claim that a broker held the user's data or completed deletion without evidence from the official process.

## Limitations

- The program is limited to eligible California residents and registered data brokers.
- Data brokers may take up to 90 days to report a status in DROP. A pending result before then does not itself justify a duplicate direct deletion request.
- Coverage, exemptions, and portal behavior may change. Stop if the live process differs materially from this profile.
- GoneBot does not decide eligibility or provide legal advice.
