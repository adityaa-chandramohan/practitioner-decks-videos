# LiveKit & the QA of Voice AI Agents — Practitioner Deck

A practitioner deck on **LiveKit** — the open-source infrastructure behind real-time voice AI (OpenAI's ChatGPT voice mode runs on it) — and how QA validates the agents built on it.

## Contents

| File | What it is |
|------|------------|
| [`LiveKit-and-the-QA-of-Voice-AI-Agents.pptx`](LiveKit-and-the-QA-of-Voice-AI-Agents.pptx) | The slide deck (PowerPoint) |
| [`LiveKit-Voice-AI-QA-Narrated.zip`](LiveKit-Voice-AI-QA-Narrated.zip) | Self-contained narrated deck — extract and open `LiveKit Voice AI QA.dc.html` in a browser to play the presentation with spoken voiceover and live captions |

▶ Prefer to watch it online? The narrated deck is hosted on my portfolio: **[adityaa-portfolio.pages.dev/decks/livekit-voice-ai-qa](https://adityaa-portfolio.pages.dev/decks/livekit-voice-ai-qa/)**

## What the deck covers

- The **STT → LLM → TTS pipeline** that powers real-time voice agents, and where each layer can fail
- A **layer-by-layer validation model** for voice AI systems
- Wiring agent traces into **Arize Phoenix** for LLM-as-judge evaluation
- **Synthetic-caller simulation** as repeatable regression suites
- The **release gates** that block a ship: latency, accuracy, safety, and conversation quality

## Tech

`Voice AI` · `LiveKit` · `WebRTC` · `Arize Phoenix` · `LLM-as-Judge` · `QA Strategy`
