# By Heart

By Heart helps you commit poems to memory and carry them forward. It combines proven memorization techniques — progressive reveal, first-letter cueing, spaced repetition, and spoken recitation — with an experience designed around the belief that a memorized poem is not an achievement to unlock but a work of art held within you, available for refuge and transcendence whenever you need it.

## Why This Exists

For most of human history, poetry was an oral art. People carried poems within them the way they carried songs — not as text to be looked up, but as language available at any moment, shaped by their own voice and breath. That practice has largely disappeared, and with it, something real has been lost.

By Heart exists to make that practice accessible again. Not as an academic exercise or a memory challenge, but as something genuinely pleasurable — a deepening relationship between a person and the poems that matter to them.

## What It Does

**Preserves poems exactly as written.** Punctuation, capitalization, spelling, spacing, and line structure are treated as immutable. The app is a scaffold around the text, never a filter on it. An e.e. cummings poem stays exactly as cummings wrote it.

**Teaches through progressive revelation.** Rather than demanding immediate recall, the app gradually removes words across practice sessions — every fifth word, then every third, then only first words, then only first letters, then nothing. Each stage builds on the last, making memorization feel like momentum rather than labor.

**Schedules review intelligently.** The SM-2 spaced repetition algorithm tracks your progress with each poem and schedules reviews at widening intervals — just before you would have forgotten. Poems you know well recede; poems that need attention surface.

**Honors the voice.** Listen to poems read aloud through text-to-speech or your own recorded reading. Recite poems and receive precise, character-level feedback on accuracy. Practice while walking with an audio-only mode that requires no screen interaction.

**Supports the ongoing relationship.** A contemplative practice mode with no scoring, no tracking, and no feedback — just you and a poem you carry within you. The app holds the poem for you whenever you want to return to it.

## Design Philosophy

The tone is reading room, not classroom. Progression feels like deepening, not leveling up. Sessions are short by design — the app encourages you to stop before fatigue, not after. Every interaction should make you want to come back.

The app does the heavy lifting so you can focus on the poetry. Input accepts pasted text, uploaded photos, and PDFs. The app handles extraction and conversion; you verify the result. Autocorrect, autocapitalize, and spellcheck are disabled throughout to protect the integrity of every character.

Mobile is the primary practice device. Poem input and verification are better on larger screens, but daily practice, recitation, and walking recitation are phone activities. Display fidelity on mobile is preserved through horizontal scroll on overflow — lines never reflow.

## Technical Details

- **Stack:** React 18, Tailwind CSS (CDN), no build system
- **Hosting:** GitHub Pages
- **Persistence:** IndexedDB (client-side, no server)
- **API integrations:** Bring-your-own-key model for speech services
  - Text-to-speech: Web Speech API (free, built-in) or ElevenLabs (premium quality)
  - Speech-to-text: OpenAI Whisper (for recitation feedback)
  - OCR: Tesseract.js (client-side, free) for photo/PDF import
- **Cost:** The core app is entirely free. Voice features use optional paid APIs at modest cost (estimated $5-10/month with active daily use).
- **Privacy:** All data stays on your device. No accounts, no cloud storage, no tracking. API keys are stored locally and never transmitted except to the API provider.

## Status

By Heart is in active development. See the [build plan](by-heart-build-plan.md) for the current roadmap.

## License

MIT

---

*"The point is that the more senses you draw on during the process of memorization, the more effective the end result — hearing the words in your mind, visualizing the imagery, copying the lines into your notebook, reasoning about how the poem's argument evolves from verse to verse, chunking words together into quotes and phrases, all of this helps, but it then also becomes more apparent that the key ingredient in memorization is time — time to read, re-read, and slowly let your thoughts steep in the words."*
