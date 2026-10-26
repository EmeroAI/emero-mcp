# Emero MCP server

**Teach your AI assistant to make pro images and video.**

Emero turns your AI assistant, like Claude or ChatGPT, into a creative director. Connect it once and ask for images, video, music or speech in plain words. It runs the model you pick: Kling 3.0, Seedance 2.5, Nano Banana Pro, GPT Image 2.5 and more.

Behind it is a second brain. Every generation teaches it something: what a model is good at, which prompt fixed a problem, which look your brand keeps. Emero saves those lessons for your brand and uses them on the next prompt, so results get better the more you make.

It starts smart. Emero is built on 6,000+ tested generations and counting, and 100+ of those workflows are public with the exact prompts and real costs at [emero.studio/workflows](https://www.emero.studio/workflows).

This repository holds the public documentation and the [MCP Registry](https://registry.modelcontextprotocol.io) metadata for Emero's hosted MCP server. The server itself is run by Emero; its source is not published here.

## Connect

| | |
|---|---|
| Server URL | `https://mcp.emero.studio/mcp` |
| Transport | Streamable HTTP (remote) |
| Sign-in | OAuth 2.1, with your Emero account |
| Registry name | `io.github.EmeroAI/emero` |
| Server card | [`/.well-known/mcp/server-card.json`](https://mcp.emero.studio/.well-known/mcp/server-card.json) |

**Claude:** Settings → Connectors → Add custom connector, paste the server URL, then sign in.

**Other MCP clients:** add a remote MCP server with the URL above. The client opens Emero's sign-in page the first time it connects.

## What it can do

| Tool | What it does |
|---|---|
| `generate` | Make an image, video clip, music track, voiceover or upscale, billed at model cost |
| `combine_videos` | Join clips into one continuous video |
| `check_generation` | Fetch the result of a running generation |
| `search_creations` | Find past generations by description |
| `view` / `inspect` | Show assets to you, or let the assistant look at them |
| `ingest_url` / `request_upload` | Bring your own images and video in as references |
| `get_settings` / `set_settings` | Read or change model, aspect ratio, duration and other settings |
| `get_emero_brain` / `save_to_emero_brain` / `manage_emero_brain` | The brand's second brain: look, rules, subjects and decisions |
| `get_pricelist` | Current price per model |
| `load_skill` | Emero's step-by-step guidance for each kind of job |

## Pricing

A flat $10/month for the second brain and the prompting workflows, plus each generation at the real model cost with no markup. New accounts start with $2 of generations free. Details: [emero.studio/pricing](https://www.emero.studio/pricing).

## Links

- Website: [emero.studio](https://www.emero.studio)
- Free workflows: [emero.studio/workflows](https://www.emero.studio/workflows)
- Support: hello@emero.studio
