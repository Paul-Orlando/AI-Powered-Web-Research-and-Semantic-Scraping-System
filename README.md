# AI Web Research Agent

## How It Works

1. Scrapes website content
2. Splits text into semantic chunks
3. Generates embeddings using OpenAI
4. Stores vectors in Pinecone
5. Retrieves relevant context
6. Produces AI-generated research summaries

AI-powered web scraping and semantic search agent built with Flowise, OpenAI, and Pinecone.

## Features

- Web scraping with Cheerio
- Semantic search using embeddings
- Pinecone vector database integration
- Retrieval-Augmented Generation (RAG)
- GPT-4o-mini powered responses
- Flowise workflow orchestration

---

## Architecture

```text
Website → Scraper → Text Splitter → OpenAI Embeddings
→ Pinecone → Retriever → GPT Agent
```

---

## Tech Stack

- Flowise
- OpenAI
- GPT-4o-mini
- text-embedding-3-small
- Pinecone
- Cheerio
- LangChain

---

## Pinecone Setup

| Setting | Value |
|---|---|
| Index Name | `web-scraping-v2` |
| Dimensions | `1536` |
| Metric | `cosine` |

---

## Installation

```bash
git clone https://github.com/yourusername/ai-web-research-agent.git
```

Import the Flowise JSON workflow and configure:

```env
OPENAI_API_KEY=
PINECONE_API_KEY=
```

---

## Example Questions

- "Summarize prompt engineering techniques"
- "Explain few-shot prompting"
- "What does the site say about chain-of-thought prompting?"

---

## Workflow

The exported Flowise workflow JSON is included in:

```text
flowise/scraper-agent.json
```
