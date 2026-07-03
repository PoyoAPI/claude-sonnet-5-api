# Claude Sonnet 5 cURL Examples

Use this request for a synchronous Claude Sonnet 5 chat completion.

```bash
export POYO_API_KEY="YOUR_POYO_API_KEY_HERE"
export POYO_BASE_URL="https://api.poyo.ai"

curl --fail-with-body --request POST \
  --url "$POYO_BASE_URL/v1/chat/completions" \
  --header "Authorization: Bearer $POYO_API_KEY" \
  --header "Content-Type: application/json" \
  --data '{
    "model": "claude-sonnet-5",
    "messages": [
      {
        "role": "system",
        "content": "You are a concise senior engineering assistant."
      },
      {
        "role": "user",
        "content": "Give me a short checklist for safely launching an AI API integration."
      }
    ],
    "max_tokens": 600
  }'
```

## Expected Response Shape

```json
{
  "code": 200,
  "data": {
    "id": "chatcmpl-example",
    "object": "chat.completion",
    "model": "claude-sonnet-5",
    "choices": [
      {
        "index": 0,
        "message": {
          "role": "assistant",
          "content": "..."
        },
        "finish_reason": "stop"
      }
    ],
    "usage": {
      "prompt_tokens": 64,
      "completion_tokens": 180,
      "total_tokens": 244
    }
  }
}
```
