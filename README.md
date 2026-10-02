# Swift on AWS Marketplace

Sample notebook and data for the UkisAI **Swift 1.5** model packages on Amazon SageMaker AI.

- `Swift-on-SageMaker.ipynb`: deploy, chat, stream, batch transform, clean up.
- `data/realtime-input.json`: sample real-time request.
- `data/batch-input.jsonl`: sample batch input (one chat request per line).

## API

`POST /invocations` takes an OpenAI-style chat completions body (`messages`, `max_tokens`, `temperature`, `top_p`, `stream`). It returns a chat completion with `choices[0].message.content` (answer), `reasoning_content` (reasoning), and `usage`.

| Model | Recommended instance | Also supported |
|---|---|---|
| Swift 1.5 27B | ml.g7e.2xlarge | ml.g5.2xlarge |
| Swift 1.5 Flash Next | ml.g7e.2xlarge | ml.g5.12xlarge |

Support: hello@ukisai.com
