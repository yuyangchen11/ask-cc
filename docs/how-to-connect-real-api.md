# How To Connect Ask CC To A Real Website

The public portfolio site can show Ask CC in two stages.

## Stage 1: Static Demo

Use a local question bank in frontend JavaScript. This is enough to show the idea, but it does not call a real model.

Best for:

- portfolio preview
- recruiter-safe demo
- no backend cost

## Stage 2: Real API

Use a backend endpoint such as Vercel Serverless Functions or Netlify Functions.

Recommended flow:

1. Put the OpenAI API key in server environment variables.
2. Never expose the API key in frontend JavaScript.
3. Store public-safe resume context and answer standards as markdown or JSON.
4. Send the user's question to the backend.
5. The backend loads Ask CC instructions and context, calls the model, and returns the answer.
6. Log only non-sensitive usage metadata.

## Repository Boundary

The public GitHub repository should include the Skill structure and public examples. Full private interview banks should stay in a private folder or private repository.
