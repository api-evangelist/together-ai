# Together AI (together-ai)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
