# Munito AI

**Open-model inference infrastructure for Europe.**

Munito AI runs the models, the document pipeline and the compute that an AI product is built on. One API and one
key reach all three, and your workspace keeps inference and storage in the EU.

Backed by Y Combinator.

## The three layers

| | |
| --- | --- |
| **Inference** | Open models behind OpenAI- and Anthropic-compatible APIs. Tool calling, structured outputs, streaming, vision and speech to text |
| **Document AI** | PDFs, scans and handwritten pages into Markdown, with tables and extracted fields |
| **Sandboxes** _(preview)_ | Cloud computers on demand. A microVM for your agents, code execution, CI, and much more |

Keep your SDK. Change the base URL and the key:

```python
import os

from openai import OpenAI

client = OpenAI(
    base_url="https://api.munito.ai/inference/v1",   # or https://api.eu.munito.ai/inference/v1
    api_key=os.environ["MUNITO_API_KEY"],
)
```

The same key starts a sandbox and reads a document.

## Private by default

Munito AI never sells customer data or trains on it. Prompts and outputs are not retained by default. The EU host
processes a request in the EU, a workspace sets where its data is stored, and the GDPR Data Processing Agreement
forms part of the Terms of Service. A US host serves the same API.

## Start here

- **[docs.munito.ai](https://docs.munito.ai)** — the quickstart, the models, the recipes and the API reference
- **[console.munito.ai/keys](https://console.munito.ai/keys)** — create a key
- **[munito.ai](https://munito.ai)** — the site, the prices and the contact form

## Open source

| Repository | What it is |
| --- | --- |
| [hermes-provider](https://github.com/munitoai/hermes-provider) | Munito AI as a model provider of Hermes Agent |
| [pi-provider](https://github.com/munitoai/pi-provider) | Munito AI as a model provider of pi |
| [openclaw-provider](https://github.com/munitoai/openclaw-provider) | Munito AI as a model provider of OpenClaw |
| [hpc-sandbox-benchmarks](https://github.com/munitoai/hpc-sandbox-benchmarks) | Sandbox benchmarks: real developer and CI tasks, measured end to end |

Claude Code, Codex, OpenCode, Hermes and pi all run on Munito AI models. See
[Integrations](https://docs.munito.ai/guides).

## Why

Munito AI was founded by the former inference lead at Mistral AI, on one belief: open and independent intelligence,
both models and inference, is key to economic growth and prosperity.

---

Security reports go to **security@munito.ai**.
