# Together AI GraphQL Schema

## Overview

This directory contains a conceptual GraphQL schema for the Together AI platform — an AI acceleration cloud that provides fast, scalable, and reliable generative-AI infrastructure. The Together API serves open-source and proprietary foundation models for chat, embeddings, vision, audio, image and video generation, fine-tuning, code execution, and dedicated GPU compute.

The schema is conceptual and maps the Together REST API surface into a unified GraphQL type system. It covers all major product areas documented at https://docs.together.ai/.

## Schema File

- `together-ai-schema.graphql` — Full GraphQL schema with 65+ named types

## Type Inventory

### Scalars
- `DateTime` — ISO 8601 timestamps
- `JSON` — Arbitrary JSON payloads (tool arguments, hyperparameters, env vars)
- `Float32` — 32-bit floats for embedding vectors

### Enums
| Enum | Description |
|------|-------------|
| `ModelType` | CHAT, COMPLETION, EMBEDDING, RERANK, IMAGE, VIDEO, AUDIO_TTS, AUDIO_STT, CODE, VISION |
| `ModelCapability` | FUNCTION_CALLING, STRUCTURED_OUTPUT, STREAMING, VISION, LONG_CONTEXT, TOOL_USE, CODE_EXECUTION, FINE_TUNABLE |
| `FineTuningStatus` | PENDING, QUEUED, RUNNING, COMPLETED, FAILED, CANCELLED |
| `ImageFormat` | PNG, JPEG, WEBP, B64_JSON |
| `EndpointStatus` | STARTING, RUNNING, STOPPED, FAILED, SCALING |
| `DeploymentStatus` | PENDING, ACTIVE, INACTIVE, DELETING, ERROR |
| `AcceleratorType` | H100_SXM, H100_PCIE, A100_SXM, A100_PCIE, B200, A10G, T4, L40S |
| `BatchStatus` | PENDING, IN_PROGRESS, COMPLETED, FAILED, CANCELLED, EXPIRED |
| `QueueStatus` | EMPTY, ACTIVE, CONGESTED, UNAVAILABLE |
| `ContentFlagType` | HATE, HARASSMENT, SELF_HARM, SEXUAL, VIOLENCE, ILLEGAL_ACTIVITY, PII |
| `FineTuningMethod` | LORA, FULL, DPO, QLORA |
| `AudioOutputFormat` | MP3, WAV, FLAC, PCM, OPUS |

### Core Model Types
| Type | Description |
|------|-------------|
| `Model` | Top-level model record with cost and availability |
| `ModelDetails` | Organization, type, capabilities, architecture, config, license |
| `ModelArchitecture` | Attention heads, hidden size, layers, vocabulary, position embeddings |
| `ModelParameters` | Total and active parameter counts, MoE expert configuration |
| `ModelConfig` | Context window, max output tokens, default sampling settings |

### Chat and Completion Types
| Type | Description |
|------|-------------|
| `ChatCompletion` | Full chat completion response with choices and usage |
| `ChatCompletionMessage` | Role-tagged message with optional tool calls |
| `ChatCompletionChoice` | Single choice with finish reason and logprobs |
| `ChatCompletionChunk` | Streaming delta chunk for real-time delivery |
| `ChatCompletionChunkChoice` | Delta choice within a stream chunk |
| `CompletionDetails` | Legacy text completion response |
| `CompletionChoice` | Single text completion choice |
| `CompletionMessage` | Message with role and content |
| `CompletionRequest` | Input parameters for text completion |
| `ToolCall` | Structured function/tool call from the model |

### Embedding Types
| Type | Description |
|------|-------------|
| `EmbeddingRequest` | Input for embedding generation |
| `EmbeddingResult` | Response containing all embedding vectors |
| `EmbeddingVector` | Single embedding with index and float array |

### Image Generation Types
| Type | Description |
|------|-------------|
| `ImageGeneration` | Image generation response with metadata |
| `ImageResult` | Single generated image (URL or base64) with seed |

### Usage and Cost Types
| Type | Description |
|------|-------------|
| `TokenUsage` | Prompt, completion, and total token counts |
| `UsageDetails` | Extended usage including image count, audio duration, and cost |
| `CostEstimate` | Pre-flight cost projection for a given model and token counts |
| `Usage` | Period-level usage summary with cost breakdown |

### Fine-Tuning Types
| Type | Description |
|------|-------------|
| `FineTuningJob` | Full job record with status, files, checkpoints, and events |
| `FineTuningDetails` | Method and hyperparameters (LoRA rank, learning rate, epochs, etc.) |
| `FineTuningStatus` | Live progress including step count and ETA |
| `FineTuningEvent` | Log event emitted during training |
| `TrainingFile` | Uploaded file record for training or validation data |
| `TrainingData` | Dataset descriptor with example count and validation split |
| `Checkpoint` | Saved checkpoint with step, epoch, and loss metrics |
| `CheckpointMetrics` | Train/validation loss and token accuracy at a checkpoint |

### Dedicated Endpoint and Deployment Types
| Type | Description |
|------|-------------|
| `Endpoint` | Named dedicated inference endpoint |
| `EndpointDetails` | Model, GPU allocation, autoscaling config, billing rate |
| `EndpointStatus` | Live replica counts and health check timestamp |
| `ModelDeployment` | Deployment binding between a model and an endpoint |
| `DeploymentConfig` | Replica bounds, scale-to-zero, autoscaling, custom domain |
| `GPUDetails` | Accelerator type, count, VRAM, NVLink, compute capability |
| `AcceleratorType` | Enum of supported GPU SKUs (H100, B200, A100, etc.) |

### Queue Types
| Type | Description |
|------|-------------|
| `Queue` | Queue record for a model with capacity |
| `QueueStatus` | Depth, throughput, estimated wait, and congestion state |
| `QueueItem` | Individual queued request with position and ETA |

### Batch Job Types
| Type | Description |
|------|-------------|
| `BatchJob` | Async batch inference job with lifecycle timestamps |
| `BatchDetails` | Input/output file IDs, model, endpoint, request counts |
| `BatchRequestCounts` | Total, completed, and failed request tallies |

### Moderation Types
| Type | Description |
|------|-------------|
| `ModerationResult` | Overall moderation decision for an input |
| `ContentFlag` | Per-category flag with score and subcategory |

### Auth and Rate Limit Types
| Type | Description |
|------|-------------|
| `APIKey` | API key record with prefix, scopes, and expiry |
| `Token` | OAuth-style access token response |
| `RateLimitInfo` | Per-model request and token limits with reset timestamps |
| `Error` | Structured API error with code, message, and type |

### Audio Types
| Type | Description |
|------|-------------|
| `AudioSpeechResult` | TTS output with URL or base64 audio content |
| `AudioTranscriptionResult` | STT transcript with optional word- and segment-level detail |
| `TranscriptionWord` | Word-level timestamp and confidence |
| `TranscriptionSegment` | Segment with token IDs, log-prob, and no-speech probability |

### Rerank Types
| Type | Description |
|------|-------------|
| `RerankResult` | Single document with relevance score |
| `RerankResponse` | Full rerank response with ordered results |

## Root Operations

### Queries
- Model catalog browsing and filtering by type and capability
- Fetching chat completion and text completion records by ID
- Embedding result retrieval
- Fine-tuning job listing, status polling, and checkpoint inspection
- Training file management
- Dedicated endpoint listing and status checks
- Queue depth and throughput monitoring
- Batch job listing and status polling
- Usage and cost reporting
- Moderation result retrieval
- API key management and rate limit inspection

### Mutations
- `createChatCompletion` — synchronous and streaming chat
- `createCompletion` — legacy text completion
- `createEmbedding` — vector embedding generation
- `createImageGeneration` — text-to-image
- `createFineTuningJob` / `cancelFineTuningJob` — training lifecycle
- `uploadTrainingFile` / `deleteTrainingFile` — dataset management
- `createEndpoint` / `updateEndpoint` / `startEndpoint` / `stopEndpoint` / `deleteEndpoint` — dedicated GPU management
- `createBatchJob` / `cancelBatchJob` — async batch inference
- `createModerationCheck` — content safety
- `createAPIKey` / `deleteAPIKey` / `rotateAPIKey` — key lifecycle

### Subscriptions
- `chatCompletionStream` — real-time token streaming for chat
- `completionStream` — real-time token streaming for text completions
- `fineTuningJobUpdated` — live training progress events
- `batchJobUpdated` — batch job status changes
- `endpointStatusChanged` — dedicated endpoint health events

## References

- Together AI Documentation: https://docs.together.ai/
- Chat Completions API: https://docs.together.ai/reference/chat-completions
- Embeddings API: https://docs.together.ai/docs/embeddings-overview
- Fine-Tuning API: https://docs.together.ai/docs/fine-tuning-overview
- Images API: https://docs.together.ai/docs/images-overview
- Dedicated Endpoints: https://docs.together.ai/docs/dedicated-endpoints-overview
- Batch API: https://docs.together.ai/docs/batch-overview
- Models API: https://docs.together.ai/reference/models
