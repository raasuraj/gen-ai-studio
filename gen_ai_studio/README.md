# GEN AI STUDIO — All-in-One AI Workspace

This version is designed as a single ChatGPT-style platform. The main chat can route normal requests to text, coding, image or video generation, while dedicated tools remain available from the sidebar.

## Included
- AI Chat / auto routing
- Prompt Studio
- AI Writer
- AI Coding
- Translator
- Image generation via OpenAI Images API
- Video generation job + polling + MP4 endpoint
- Basic TXT/MD/CSV document reading into AI
- Browser text-to-speech
- Responsive desktop/mobile UI

## Render setup
1. Create a Render Web Service from this repository.
2. Root Directory: leave blank.
3. Build Command: leave blank.
4. Start Command: `npm start`
5. Add Environment Variable: `OPENAI_API_KEY` = your OpenAI API key.
6. Optional: `OPENAI_MODEL` (default `gpt-5.6-luna`), `OPENAI_IMAGE_MODEL` (default `gpt-image-2`), `OPENAI_VIDEO_MODEL` (default `sora-2`).

Do NOT put the API key into frontend JavaScript or commit it to GitHub.

## Important
Actual model availability, API access, pricing and limits depend on the OpenAI account/API access. Video generation is asynchronous, so the UI waits for the job to complete.
PDF/DOCX/OCR extraction is intentionally separated from the simple text-file reader; production PDF/Word/OCR processing needs a file-capable backend/model integration.
