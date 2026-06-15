# Together AI (together-ai)

Together AI is an AI acceleration cloud delivering fast, scalable, and reliable generative-AI infrastructure. The Together API serves open-source and proprietary foundation models for chat, embeddings, vision, audio, image and video generation, fine-tuning, code execution, and dedicated GPU compute.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/apis.yml)

## Tags

- AI
- LLM
- Inference
- Foundation Models
- GPU
- Open Source AI

## Timestamps

- **Created:** 2026-05-08
- **Modified:** 2026-05-29

## APIs

### Together Chat Completions API

OpenAI-compatible chat completions across hundreds of open-source and proprietary models including Llama, Qwen, DeepSeek, GLM, Kimi, and Mistral families with streaming, tool use, and structured outputs.

- **Human URL:** [https://docs.together.ai/reference/chat-completions](https://docs.together.ai/reference/chat-completions)
- **Base URL:** `https://api.together.ai/v1`

#### Tags

- Chat
- Completions
- LLM

#### Properties

- [Documentation](https://docs.together.ai/docs/chat-overview)
- [API Reference](https://docs.together.ai/reference/chat-completions)
- [OpenAPI](openapi/together-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/together-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/together-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/together-ai-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)

### Together Completions API

Legacy text-completion endpoint for non-chat models, OpenAI-compatible.

- **Human URL:** [https://docs.together.ai/reference/completions](https://docs.together.ai/reference/completions)
- **Base URL:** `https://api.together.ai/v1`

#### Tags

- Completions
- LLM

#### Properties

- [API Reference](https://docs.together.ai/reference/completions)
- [OpenAPI](openapi/together-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/together-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/together-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/together-ai-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)

### Together Embeddings API

Generates dense vector embeddings (e.g., multilingual-e5-large-instruct, BGE) for retrieval, RAG, and semantic-search workflows.

- **Human URL:** [https://docs.together.ai/docs/embeddings-overview](https://docs.together.ai/docs/embeddings-overview)
- **Base URL:** `https://api.together.ai/v1`

#### Tags

- Embeddings
- Vector
- Retrieval

#### Properties

- [Documentation](https://docs.together.ai/docs/embeddings-overview)
- [API Reference](https://docs.together.ai/reference/embeddings)
- [OpenAPI](openapi/together-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/together-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/together-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Together Rerank API

Reranks candidate passages against a query using cross-encoder models for higher-quality retrieval and RAG.

- **Human URL:** [https://docs.together.ai/docs/rerank-overview](https://docs.together.ai/docs/rerank-overview)
- **Base URL:** `https://api.together.ai/v1`

#### Tags

- Rerank
- Retrieval
- RAG

#### Properties

- [Documentation](https://docs.together.ai/docs/rerank-overview)
- [OpenAPI](openapi/together-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/together-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/together-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Together Images API

Text-to-image generation across FLUX.1, FLUX.2, Nano Banana Pro, Stable Diffusion, and Dreamshaper model families.

- **Human URL:** [https://docs.together.ai/docs/images-overview](https://docs.together.ai/docs/images-overview)
- **Base URL:** `https://api.together.ai/v1`

#### Tags

- Images
- Generation
- Diffusion

#### Properties

- [Documentation](https://docs.together.ai/docs/images-overview)
- [API Reference](https://docs.together.ai/reference/images-generations)
- [OpenAPI](openapi/together-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/together-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/together-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Together Video API

Text-to-video and image-to-video generation across multiple quality and duration tiers.

- **Human URL:** [https://docs.together.ai/docs/video-overview](https://docs.together.ai/docs/video-overview)
- **Base URL:** `https://api.together.ai/v1`

#### Tags

- Video
- Generation
- Multimodal

#### Properties

- [Documentation](https://docs.together.ai/docs/video-overview)
- [OpenAPI](openapi/together-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/together-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/together-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Together Audio API

Text-to-speech (MiniMax Speech, Cartesia Sonic, Kokoro, Orpheus) with sub-250ms latency, and speech-to-text (Whisper Large v3, Parakeet) with 40+ language support.

- **Human URL:** [https://docs.together.ai/docs/audio-overview](https://docs.together.ai/docs/audio-overview)
- **Base URL:** `https://api.together.ai/v1`

#### Tags

- Audio
- Speech
- TTS
- STT

#### Properties

- [Documentation](https://docs.together.ai/docs/audio-overview)
- [OpenAPI](openapi/together-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/together-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/together-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/together-ai-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)

### Together Vision API

Multimodal vision and document understanding using models such as Qwen 3.5 (397B and 9B) and Kimi K2.5.

- **Human URL:** [https://docs.together.ai/docs/vision-overview](https://docs.together.ai/docs/vision-overview)
- **Base URL:** `https://api.together.ai/v1`

#### Tags

- Vision
- Multimodal
- Documents

#### Properties

- [Documentation](https://docs.together.ai/docs/vision-overview)
- [OpenAPI](openapi/together-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/together-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/together-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Together Fine-Tuning API

Supervised fine-tuning (LoRA and full) and DPO across the Together model catalog with managed training jobs and one-click deployment.

- **Human URL:** [https://docs.together.ai/docs/fine-tuning-overview](https://docs.together.ai/docs/fine-tuning-overview)
- **Base URL:** `https://api.together.ai/v1`

#### Tags

- Fine-Tuning
- LoRA
- Training

#### Properties

- [Documentation](https://docs.together.ai/docs/fine-tuning-overview)
- [API Reference](https://docs.together.ai/reference/fine-tunes-create)
- [OpenAPI](openapi/together-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/together-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/together-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Together Files API

Upload, list, retrieve, and delete training datasets and batch input files.

- **Human URL:** [https://docs.together.ai/reference/files](https://docs.together.ai/reference/files)
- **Base URL:** `https://api.together.ai/v1`

#### Tags

- Files
- Storage

#### Properties

- [API Reference](https://docs.together.ai/reference/files)
- [OpenAPI](openapi/together-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/together-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/together-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Together Models API

Lists hundreds of available models with metadata, capabilities, context window, and pricing.

- **Human URL:** [https://docs.together.ai/reference/models](https://docs.together.ai/reference/models)
- **Base URL:** `https://api.together.ai/v1`

#### Tags

- Models
- Catalog

#### Properties

- [API Reference](https://docs.together.ai/reference/models)
- [OpenAPI](openapi/together-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/together-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/together-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Together Batch API

Asynchronous batch inference with up to 50% discount over synchronous rates; fetch results when complete.

- **Human URL:** [https://docs.together.ai/docs/batch-overview](https://docs.together.ai/docs/batch-overview)
- **Base URL:** `https://api.together.ai/v1`

#### Tags

- Batch
- Async

#### Properties

- [Documentation](https://docs.together.ai/docs/batch-overview)
- [OpenAPI](openapi/together-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/together-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/together-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Together Code Interpreter API

Sandboxed Python execution alongside model calls for tool-using agents and code workflows.

- **Human URL:** [https://docs.together.ai/docs/code-interpreter-overview](https://docs.together.ai/docs/code-interpreter-overview)
- **Base URL:** `https://api.together.ai/v1`

#### Tags

- Code
- Execution
- Sandbox

#### Properties

- [Documentation](https://docs.together.ai/docs/code-interpreter-overview)
- [OpenAPI](openapi/together-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/together-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/together-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Together Evaluations API

LLM-as-judge evaluations with automated scoring and reports for model comparisons.

- **Human URL:** [https://docs.together.ai/docs/evaluations-overview](https://docs.together.ai/docs/evaluations-overview)
- **Base URL:** `https://api.together.ai/v1`

#### Tags

- Evaluations
- Quality

#### Properties

- [Documentation](https://docs.together.ai/docs/evaluations-overview)
- [OpenAPI](openapi/together-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/together-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/together-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Together Dedicated Endpoints API

Provision and manage dedicated GPU-backed inference endpoints (H100, B200) with hourly billing for predictable performance and isolation.

- **Human URL:** [https://docs.together.ai/docs/dedicated-endpoints-overview](https://docs.together.ai/docs/dedicated-endpoints-overview)
- **Base URL:** `https://api.together.ai/v1`

#### Tags

- Dedicated
- Endpoints
- Deployment

#### Properties

- [Documentation](https://docs.together.ai/docs/dedicated-endpoints-overview)
- [OpenAPI](openapi/together-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/together-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/together-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/togethercomputer)
- [LinkedIn](https://www.linkedin.com/company/togethercomputer)
- [Website](https://www.together.ai/)
- [Documentation](https://docs.together.ai/)
- [Plans](plans/together-ai-plans-pricing.yml)
- [Rate Limits](rate-limits/together-ai-rate-limits.yml)
- [Fin Ops](finops/together-ai-finops.yml)
- [L L Ms Txt](https://docs.together.ai/llms.txt)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
