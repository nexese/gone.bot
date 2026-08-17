# 5. Approval and execution

## Obtain approval at the action boundary

Ask for explicit approval immediately before sending an email, submitting a form, uploading a document, or making another external disclosure. Approval applies only to the previewed action. Prior enthusiasm, general consent, or approval for another broker is insufficient.

Approval is a conversational response to the agent, not a control on the broker's website. End every approval preview with a direct instruction such as: `Reply "approve" in this conversation to authorize this action, or reply with changes or "cancel".` Do not imply that an approval button exists in the portal or desktop client. If the live site also has a button such as **I accept** or **Submit**, identify it separately as the site control the harness will use after conversational approval.

## Use harness-owned connectors

After approval, use the current harness's browser or email connector. GoneBot provides no connector implementation or credential store. Never ask the user to install or start a GoneBot service or MCP server.

If the connector is unavailable or the live flow differs from the preview, stop. Provide the user with the official destination and prepared text for manual completion.

## Record the observed result

Update the progress file with one of these distinct states:

- `drafted`
- `approved`
- `submitted`
- `acknowledged`
- `attention-needed`
- `broker-reported-complete`
- `verified`
- `denied`
- `failed`
- `unknown`

Record the date, channel, destination, and a minimal evidence reference. An attempted submission with no reliable result is `unknown`, not `submitted`; do not retry blindly.
