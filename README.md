# RecapAI Myanmar — MVP Prototype

A Burmese-first movie recap studio UI. This prototype includes upload UI, recap settings, editable Burmese script, voice studio, projects, and export controls.

## Run
Open `index.html` in a browser. No build step is required.

## Production architecture
- Frontend: React/Next.js + TypeScript
- Auth/database/storage: Supabase or PostgreSQL + S3-compatible storage
- AI: server-side LLM for recap/script/translation
- Transcription: Whisper-compatible speech-to-text
- Burmese TTS: a provider with Burmese neural voices
- Media: FFmpeg worker for cutting, subtitles, mixing, and MP4 rendering
- Queue: Redis/BullMQ or managed job queue
- Payments: age-appropriate account/guardian-managed billing if monetized

## Important
The current buttons are a UI prototype; no external AI keys are embedded. For a real product, keep API keys server-side and process only video/material the user is authorized to use.
