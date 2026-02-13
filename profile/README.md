# Welcome to Prove AI

Prove AI is building an observability-first foundation for production generative AI systems. Our long-term goal is to help engineering teams understand, diagnose, and ultimately remediate failures across complex AI pipelines—LLM inference, retrieval, agent orchestration, and everything in between.

This organization hosts Prove AI v0.1, the first building block toward that vision.

## What is Prove AI v0.1?

Prove AI v0.1 is an opinionated observability pipeline for generative AI workloads. It focuses on collecting, exporting, and structuring telemetry from AI systems so teams can reason about their behavior in production environments.

Specifically, v0.1 provides:

- A containerized, OpenTelemetry-based telemetry pipeline
- Preconfigured collection of traces, metrics, and logs for AI workloads
- Instrumentation patterns tailored to LLM inference, RAG pipelines, embeddings, and agent-based systems
- Compatibility with standard backends including Prometheus and other OpenTelemetry consumers

This release is intentionally scoped to making AI systems observable first; without high-quality telemetry, higher-level diagnosis and remediation are not possible.

## Get Started

To learn more about Prove AI, see [proveai.com](https://proveai.com).

To deploy the observability stack locally, start with the [quickstart guide](https://github.com/prove-ai/observability-pipeline/blob/main/docs/guides/quick-start.md). A working pipeline can be running in under an hour. You may also find [this accompanying video](https://app.frame.io/reviews/a04b5d96-4ef3-4ab0-b423-50c68ad86911/392dfc5f-7592-4511-806c-ee0229b93f74?version=a8945bb3-bf0a-4225-bb7e-39d70055023a) helpful (the main demo begins at 1:12), as it covers much of the quickstart and some of the vLLM guide, and includes a basic walkthrough of the Prove AI Dashboard. 

For a detailed overview of the platform's architecture and design rationale, read the [technical whitepaper](https://github.com/prove-ai/observability-pipeline/blob/main/docs/prove-technical-whitepaper.mdx).

## Repositories

- [observability-pipeline](https://github.com/prove-ai/observability-pipeline): the core containerized stack—OpenTelemetry Collector, Prometheus, and GenAI-optimized configurations. Start here.
- [docs](https://github.com/prove-ai/observability-pipeline/tree/main/docs): technical whitepaper, UI walkthrough, and an integration guide for vLLM (more will be coming in the future).

## Guides

- [Quick Start](https://github.com/prove-ai/observability-pipeline/blob/main/docs/guides/quick-start.md): deploy the full observability stack with Docker Compose.
- [vLLM Integration](https://github.com/prove-ai/observability-pipeline/blob/main/docs/guides/vllm-guide.md): instrument vLLM inference endpoints with Prometheus and OpenTelemetry.
- [UI Walkthrough](https://github.com/prove-ai/observability-pipeline/blob/main/docs/ui-walkthrough.mdx): navigate the Prove AI dashboard, evaluations, guardrails, and configuration interfaces.
