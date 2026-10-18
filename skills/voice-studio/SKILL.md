---
name: voice-studio
description: "Use the official local VoiceStudio API to generate authorized spoken narration or dub audio for creative media projects."
triggers:
  - "voice studio"
  - "voice clone narration"
  - "local text to speech"
od:
  mode: utility
  category: audio-music
  upstream: "https://github.com/debpalash/VoiceStudio"
---

# VoiceStudio — optional voice synthesis service

Use this when authorized narration, multilingual voiceover or text-to-speech is needed. The upstream app supplies the engines and media; this skill is a catalog entry only.

A running VoiceStudio instance exposes `GET /v1/audio/voices` and `POST /v1/audio/speech` at `http://127.0.0.1:3900/v1`. Claude/Codex can use VoiceStudio's official MCP server at `http://127.0.0.1:3900/mcp/` when the app is actually running. The sibling `codex-video-tools/scripts/voicestudio_speech.py` optional bridge uses this provider contract to generate a WAV for the existing FFmpeg timeline.

Do not clone or imitate someone's voice without appropriate permission, store recordings/voice profiles in Git, or make a loopback service public. A remote provider requires a private authenticated HTTPS connection and available compute. The upstream code is AGPL-3.0 and the engine/model licenses vary; **link to the provider instead of vendoring its source here**.

Sources: https://github.com/debpalash/VoiceStudio and https://github.com/debpalash/VoiceStudio/blob/main/docs/agentic-voice.md. This entry is not a service install.
