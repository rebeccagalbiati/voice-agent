# Rebecca's voice agent

A voice agent that welcomes visitors into the world of **Rebecca Galbiati**, Creative Director & Event Producer based in Paris, and answers their questions about her work, her events and her approach.

It speaks **English, French and Italian**, replying in whatever language the visitor uses. Its voice is female, professional, witty and welcoming, with a slight Italian accent in English and French.

## Try it

1. Open the live page: **https://<username>.github.io/voice-agent/**
2. Paste a Gemini API key (free at [Google AI Studio](https://aistudio.google.com/apikey)) and press **Begin**.
3. Tap the circle and speak, or write in the field below it. Works best in **Chrome**.

## How it works

| Step | Technology |
|---|---|
| Listen | Web Speech API (`SpeechRecognition`), in the browser |
| Think | Gemini API (`generateContent`), with a persona and Rebecca's profile as the system instruction, and the conversation history |
| Speak | Gemini text-to-speech (female voice, style and accent set by prompt); falls back to the browser's voice if unavailable |

Everything is in a single file, `index.html`. The agent's knowledge and personality are at the top of the script (`PERSONA`), so they are easy to update.

## About the API key

The key is **not** stored in this repository. Each visitor types their own key into the page, and it is saved only in their own browser (localStorage).

Design: ivory, ink and pink palette with Fraunces and Cormorant Garamond, matching [rebeccagalbiati.com](https://rebeccagalbiati.com).
