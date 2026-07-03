# Production Notes

Use this checklist before putting claude-sonnet-5 chat completions into a user-facing product.

## API Key Safety

- Store `POYO_API_KEY` in server-side environment variables.
- Never send the key to browser code or mobile clients.
- Do not print `Authorization` headers in logs.

## Request Handling

- Validate incoming messages before calling the model.
- Set `max_tokens` to control response length and cost.
- Keep private user prompts out of logs unless your product policy allows them.

## Reliability

- Use request timeouts in your application.
- Retry only transient transport failures.
- Return concise errors to the client without exposing upstream details.
