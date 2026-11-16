# Verified report delivery

Use the host's existing approved scheduling, storage and email tools. The skill supplies the workflow contract, not a standalone scheduler or mail server. Missing connectors must be disclosed; never fabricate delivery evidence.

## Close timing and ownership

Resolve actual trading date and official regular close, including holidays, early closes and daylight-saving changes. Never generate a completed-close report before the session closes. Recheck extraordinary closures when uncertain. Use one run owner and one durable state directory per report kind and market date. Do not silently take over an expired owner or backfill a missed round without authorization.

Save trigger, actual start, source sampling, generation and delivery times separately. Commit collection, research and validation artifacts with fingerprints. Resume matching completed stages after interruption; keep source evidence immutable. Record each model's original output or failure alongside the final assistant synthesis.

## Sending contract

1. Check local delivery records and the actual email provider for the exact authorized recipient, report type and market date. Daily briefs use their specified local reporting date; close reports use the exchange date.
2. Validate the complete rendered report and factual blockers. If blocked, retain the report and explain the unresolved stage. Do not clear blockers merely to permit sending.
3. Immediately before sending, repeat the provider duplicate check and persist a sending/unknown intent under the run lock. Send the validated complete body only once.
4. Persist the actual returned message ID immediately, even if the execution lease expires after the send. A timeout or missing response means unknown, not permission to resend. Search provider records to reconcile.
5. Read that actual message's full body and SENT state. Compare recipient, subject and the complete rendered body, not just a snippet or success flag. Record the receipt and explicit report date. If receipt reading fails, preserve the actual ID and resume verification without sending again.
6. Only after the complete evidence matches, report the artifact link and actual delivery time. A notification popup requires separate observation; do not infer it from email success.

Public skill installation does not grant permission to email anyone. Reuse the user's explicit authorized recipient and task scope; never embed personal recipients or account credentials in a shared skill.
