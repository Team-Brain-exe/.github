# Orbitveil

### Privacy-Preserving Browser AI Agent

Orbitveil is a privacy-preserving browser AI agent designed for on-device visual perception. It uses a local vision model to detect and redact sensitive information—such as faces, passwords and personally identifiable information (PII)—from screen content before the data is sent to a server-side vision-language model (VLM) for reasoning and action planning.

The project is built for **Smart India Hackathon 2026 – Problem Statement 26171 (ISRO)**.

## Main Components

- **Browser Extension (`extension/`)** — Chrome Manifest V3 extension for local vision processing, sensitive-data redaction and action execution.
- **Backend Server (`server/`)** — FastAPI backend for server-side VLM integration and API handling.
- **Shared (`shared/`)** — Shared action-schema contract between the extension and backend.
- **Demo (`demo/`)** — Test page and demonstration scripts.
- **Evaluation (`eval/`)** — Benchmarking and evaluation against SIH requirements.
- **Documentation (`docs/`)** — Architecture and project documentation.

## Key Features

- On-device visual perception
- Sensitive-information detection and redaction before server transmission
- Face and password protection
- Browser-based AI agent architecture
- Server-side VLM reasoning
- Browser action execution
- Shared action-schema contract
- Evaluation and benchmarking support
- Docker-based deployment support

## Technology Stack

| Component | Technologies |
|---|---|
| Browser Extension | JavaScript, Chrome Manifest V3, MediaPipe Tasks Vision, esbuild, ES Modules |
| Backend | Python, FastAPI, Uvicorn, Pydantic |
| AI / VLM | Groq |
| Image Processing | Pillow |
| HTTP / Configuration | Requests, python-dotenv, python-multipart |
| Infrastructure | Docker, Docker Compose |

## Architecture

```text
User Screen / Browser
        |
        v
Browser Extension (Chrome MV3)
  - Local visual processing
  - Sensitive-data detection
  - Redaction
  - Action execution
        |
        | Sanitized data
        v
FastAPI Backend
  - API handling
  - VLM integration
  - AI reasoning / action planning
        |
        v
Response / Action
        |
        v
Browser Extension
```

## Repository

[Orbitveil-SIH / Orbitveil](https://github.com/Orbitveil-SIH/Orbitveil)
