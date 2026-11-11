# ISHARA

### Two-Way Indian Sign Language–Speech Translation Kiosk

ISHARA is a two-way Indian Sign Language (ISL)–speech translation kiosk designed for frontline government service points such as RTOs, Aadhaar/PAN centres and Common Service Centres (CSCs). It enables real-time communication between citizens who use sign language and staff who communicate through speech.

The system uses two frontend applications: a citizen-facing camera interface for recognizing signs and a staff-facing voice interface for speech communication. A central session server synchronizes both sides in real time, while a Python model service handles the AI/model-processing layer.

## Main Components

- **Vision Lab** — Citizen-facing camera interface for sign recognition.
- **Voice Lab** — Staff-facing voice interface for speech communication.
- **Session Server** — Node.js service coordinating sessions and real-time communication.
- **Model Service** — Python service responsible for AI/model processing.

## Technology Stack

| Component | Technologies |
|---|---|
| Frontend applications | JavaScript / TypeScript |
| Frontend package manager | pnpm |
| Session server | Node.js |
| Real-time communication | Socket.IO |
| AI / Model service | Python |
| Model API | FastAPI, Uvicorn |
| Computer vision | Camera-based Indian Sign Language recognition |
| Speech interface | Microphone / speech communication |

## Architecture

Two frontend applications (Vision Lab and Voice Lab) communicate through a Node.js session server using Socket.IO. A Python model service provides the AI/model-processing layer.

## Repository

[Team-Brain-exe / ISHARA](https://github.com/Team-Brain-exe/ISHARA)
