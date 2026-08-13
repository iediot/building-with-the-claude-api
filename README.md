# Building with the Claude API

Notebooks from [Anthropic Academy's course of the same name](https://anthropic.skilljar.com/claude-with-the-anthropic-api)
— 11 modules, ~84 lessons.

## Setup

```bash
pip install anthropic python-dotenv jupyter
```

Put your key in a `.env` here — every notebook calls `load_dotenv()`, so `Anthropic()` picks it up:

```
ANTHROPIC_API_KEY=your-key-here
```

Note that in order to get an API key to work, usage credits are needed.

The model is set per notebook, so they don't all use the same one — change the `model` variable
at the top to switch.

## What the course covers

**Accessing Claude with the API.** The messages list and multi-turn conversations (the API is
stateless — you resend the whole conversation each turn), system prompts, temperature, response
streaming, and getting structured data back via message prefilling and stop sequences.

**Prompt evaluation.** The eval workflow: generating a test dataset, running a prompt across it,
then grading the results — both model-based and code-based.

**Prompt engineering.** Being clear, direct, and specific; structuring prompts with XML tags;
providing examples.

**Tool use.** Tool functions and schemas, handling message blocks, sending tool results back,
multi-turn and multi-tool flows, fine-grained tool calling, plus the built-in text-edit and
web-search tools.

**RAG and agentic search.** Text chunking, embeddings, the full retrieval flow, BM25 lexical
search, and multi-index pipelines.

**Features of Claude.** Extended thinking, image and PDF support, citations, prompt caching,
code execution and the Files API.

**Model Context Protocol.** Building MCP servers and clients — defining tools, resources, and
prompts, and using the server inspector.

**Anthropic apps.** Claude Code setup and usage, extending it with MCP servers, and computer use.

**Agents and workflows.** Parallelization, chaining, and routing workflows; agents with tools;
environment inspection; and when a workflow beats an agent.
