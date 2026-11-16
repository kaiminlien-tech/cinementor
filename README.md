# CineMentor — bilingual film & language mentor

A responsive English/Hebrew learning chatbot prototype for film-based language learning.

## What's included
- Bilingual interface (English/Hebrew) and learner profile settings.
- Prepared activity starters for vocabulary, speaking, listening, writing, Maslow and Bronfenbrenner.
- Local demo fallback replies.
- Optional live AI endpoint using the OpenAI Responses API.
- Server-side API key handling (the key is never placed in browser JavaScript).

## Run locally
1. Install Node.js (LTS).
2. Open this folder in a terminal.
3. Run `npm install`.
4. Run `npx vercel dev`.
5. Open the local URL shown by Vercel.

Without an API key, the prepared demo mode still works.
To enable AI replies locally, set `OPENAI_API_KEY` in your terminal environment before starting the dev server. Never put the key in `index.html`, `script.js`, or any public repository.

## Deploy for a shareable link (Vercel)
1. Create a GitHub account if you do not have one.
2. Create a new **private** GitHub repository named `cinementor`.
3. Upload all files and the `api` folder from this project ZIP.
4. Sign in to Vercel and choose **Add New → Project**.
5. Import your `cinementor` GitHub repository and deploy.
6. In Vercel → Project → Settings → Environment Variables, add:
   - `OPENAI_API_KEY` = your secret API key
   - Optional: `OPENAI_MODEL` = `gpt-5.5`
7. Redeploy after adding the environment variable.
8. Copy the Vercel production URL and submit it under **Link to your Bot**.

The live AI feature requires an OpenAI API key and API usage may incur charges. ChatGPT subscriptions and API billing are separate. Keep the repository private if it contains coursework drafts or personal material, and never share your API key.

## Rubric alignment
- Maslow (45): basic-needs check-in, emotional safety, belonging, confidence/goal-setting and creative growth activities.
- Bronfenbrenner (40): personalized interaction, home/school/peer connections, school/community influences, and culturally inclusive activities.
- Design/functionality (15): responsive bilingual interface, activity buttons, accessible chat feedback and optional live AI responses.

This project is an educational demo, not a clinical or counselling service. It does not collect or store learner chat history.
