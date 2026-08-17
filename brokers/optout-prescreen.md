# OptOutPrescreen.com

- ID: `optout-prescreen`
- Category: multi-company prescreen opt-out mechanism
- Jurisdictions: United States
- Review status: reviewed guidance
- Last reviewed: 2026-08-17

## Official sources

- Official industry site: <https://www.optoutprescreen.com/>
- Choice form: <https://www.optoutprescreen.com/form>

## Supported goals

- `opt-out` — stop Equifax, Experian, Innovis, and TransUnion from including a matched credit file in lists used for firm offers of credit or insurance for five years through the electronic option, or permanently after completing the postal form.

## Channels and required capabilities

- Channel: official browser form; permanent opt-out also requires printing and postal mail
- Harness capabilities: browser and filesystem; printing, signature, sensitive entry, and mailing are user-handled
- Destination: OptOutPrescreen.com

## Minimum known fields

The live form controls. It says an SSN can help match a file but processing may be attempted without it. The user decides and enters any SSN directly; it is never copied into chat or progress.

## Procedure

1. Explain that this stops specified prescreen lists; it does not delete or freeze a credit report and does not stop every marketing offer.
2. Compare the five-year electronic and permanent postal options.
3. Preview the selected option, fields, and channel; obtain approval.
4. The user enters sensitive values and submits or mails the permanent form.

## Manual checkpoints

- Sensitive identifiers, CAPTCHA, printing, signature, postage, and final submission are user-handled.

## Evidence and status interpretation

Electronic confirmation means the five-year request was accepted for matching. Permanent status requires the signed form to be mailed and processed. Neither outcome is deletion or a security freeze.

## Limitations

- Coverage is limited to prescreen lists from the four named consumer reporting companies.
- A company must be able to match a credit file for the choice to apply.
