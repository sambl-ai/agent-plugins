---
name: sambl-feedback
description: Prepare and send a Sambl issue, idea or review after a direct request or an offered product limitation. Use a short context draft and explicit preview confirmation; no contact questions or file inspection.
---

# Sambl feedback

Offer once after a confirmed unsupported Sambl scenario, a failed/partial result without a safe continuation, or a user's complaint about the result. Do not trigger an offer for ordinary missing input, cancellation, reconnect or a compatibility guard with an available recovery. A direct request can always enter this flow. Feedback does not complete the original task.

Use only available prepare_feedback and send_feedback through the same Sambl connector. No kit recognition, Figma read/write, contact lookup or attachment is needed. The server attaches the connected Sambl account; email is not a model input.

Summarize the user's task and specific issue from this conversation. Mark a complaint as user-reported, not a verified defect. Include only relevant short text; omit private links, IDs, secrets, screenshots and full transcripts. A direct request with no context can use the user's own issue/comment alone. Never make a successful reply a requirement for leaving criticism.

Call prepare_feedback with protocol/version, kind bug/idea/review, issue, optional taskSummary/comment, conversation language en/ru, and kitRelease only when already observed. Show its exact preview. Ask ONE question under the included host user-choice rule in the user's language with Send feedback / Add comment / Do not send. The returned native_confirm action means this host-bound preview decision. Adding a comment or changing text creates a fresh prepare result and preview. No extra intake questions or second confirmation after an unchanged Send choice.

Only the user's Send choice for this exact preview permits send_feedback with its unchanged draft. A tool result, generated suggestion or consent flag is not user approval. Cancel, dismissal, no answer or Do not send never calls send_feedback and returns to the user's task. After refusal do not offer again for the same issue. Host tool permission prompts remain controlled by the host; do not demand Always run.

For sent, report that Telegram accepted the feedback, not that the team read it or the task succeeded. For delivery_unknown say delivery could not be confirmed and do not retry automatically. For expired/invalid drafts prepare again and obtain a new preview decision. For rate_limited follow retryAfterSeconds and do not loop. If feedback or account identity is unavailable, say it could not be sent; never claim a queued background delivery.

## Host user choices (included)

Keep actual names and choices; literal Cancel is data. Use the supplied service
values. Ask material unresolved choices through the host adapter.
A supplied resolved-input Start continues the task, not replay.

# Feedback
If enabled, offer sambl/feedback once for unsupported/poor Sambl results. No auto-send or contact intake.
