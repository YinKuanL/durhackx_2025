# I/We — Multi-Agent AI Collaboration Platform

**3rd Place — DurHack 2025**

I/We is a hackathon-built multi-agent AI collaboration platform for solo work. It gives a user a panel of specialized local AI assistants that can brainstorm, critique, plan, and help solve tasks together instead of acting like a single chatbot.

## What it does

- Coordinates multiple AI agents in one collaborative workspace.
- Supports brainstorming, coding help, planning, research, and problem solving.
- Runs local models through Ollama for fast iteration during development.
- Combines a React/Next.js frontend with a Flask backend API.

## Tech stack

- Frontend: Next.js, React, TypeScript, Tailwind CSS
- Backend: Python, Flask
- Local AI runtime: Ollama
- Models used during the hackathon: Llama 2, Llava, Mistral, Orca 2, Qwen 2.5

## Quick start

Install the Python dependencies:

```bash
pip install -r requirements.txt
```

Install the frontend dependencies:

```bash
npm install
```

Install the local Ollama models used by the app:

```bash
ollama pull llama2
ollama pull llava:latest
ollama pull mistral
ollama pull orca2
ollama pull qwen2.5
```

Start the backend API:

```bash
cd src/api
flask run --debug
```

In a second terminal, start the frontend from the repository root:

```bash
npm run dev
```

Open the local app at the URL printed by Next.js, usually `http://localhost:3000`.

## Repository structure

```text
src/
  api/        Flask backend API
  frontend/   React/Next.js frontend
public/       Static assets
```

## Notes

This was built during DurHack 2025 as a prototype for collaborative AI workflows. Future work could improve agent coordination, persistent memory, task-specific specialists, and deployment support.
