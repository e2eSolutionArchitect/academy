# 🤖 AI Builder Career Transformation Program
---

> **Program Duration:** 13 Weeks | **Schedule:** 3 Days/Week × 3 Hours/Day = **117 Contact Hours**
> **Format:** Hands-on Coding + Whiteboarding Sessions
> **Target Learner:** Software Engineers transitioning to AI/Agent development
> **Goal:** Design, Build, Deploy, Monitor & Debug production-standard AI applications and agentic workflows

---
<img width="1376" height="768" alt="Gemini_Generated_Image_ilqm0ilqm0ilqm0i" src="https://github.com/user-attachments/assets/3969f1a5-906a-44dc-9c00-a0e93cc00dd2" />

## Program Overview

---

## 🏗️ The Evolving Project: **AURA** — *Autonomous Unified Research Assistant*

Throughout the entire program, you will build a single evolving project that grows in capability and production-readiness with each module. By the end, AURA will be a deployed, monitored, scenario-specific AI assistant with RAG, tools, evaluation, observability, and documented production trade-offs.

| Module | AURA Evolution Stage |
|--------|---------------------|
| Module 1 | AURA v0.1 — Basic prompt-powered chatbot |
| Module 2 | AURA v0.2 — Multi-model, token-aware assistant |
| Module 3 | AURA v0.3 — RAG-enabled knowledge assistant |
| Module 4 | AURA v0.4 — Evaluated, tool-using agent |
| Module 5 | AURA v0.5 — Role-based workflow with memory and guardrails |
| Module 6 | AURA v1.0 — Production-deployed, monitored system |
| Capstone | AURA Enterprise — Scenario-specific production portfolio project |

---

## Scope Calibration & Career Outcome

This program is intentionally hands-on and career-oriented. The core outcome is not to sample every AI tool, but to graduate with a credible production portfolio project: an evaluated, observable, secure AI assistant with RAG, tools, deployment, and clear documentation.

**Primary stack for the required path:**
- Python, FastAPI, Pydantic, pytest
- OpenAI and Anthropic SDKs using current generally available models
- Qdrant as the primary vector database
- LangGraph for agent workflow orchestration
- Langfuse as the primary observability layer
- Docker, GitHub Actions, and one cloud provider: AWS or Azure

**Optional / advanced stretch topics:**
- LangSmith in addition to Langfuse
- vLLM, TGI, quantization, GPU serving
- Multi-cloud deployment
- Advanced RAG patterns such as RAPTOR and knowledge graphs
- Full autonomous multi-agent debate systems

**Career targets supported by this program:**
- AI Engineer
- Generative AI Application Developer
- RAG Engineer
- Agentic Systems Developer
- LLMOps / AgentOps Engineer
- AI Solutions Engineer

Each module should produce portfolio artifacts: GitHub commits, README updates, architecture diagrams, evaluation reports, cost reports, demo screenshots, and short demo videos.

---

## 📅 Session Schedule & Structure

The program contains 39 instructor-led sessions. Each 3-hour session follows this rhythm:

```
┌─────────────────────────────────────────────────────┐
│  0:00 – 0:30  │  Concept Whiteboarding & Theory     │
│  0:30 – 1:00  │  Guided Coding / Live Demo          │
│  1:00 – 2:30  │  Hands-on Lab / AURA Evolution      │
│  2:30 – 3:00  │  Review, Debug & Retrospective      │
└─────────────────────────────────────────────────────┘
```

---

# MONTH 1 — Foundations, Prompt Engineering & AI Integration

> **Theme:** Understand the building blocks. Wire up your first AI-powered application.

---

## MODULE 1: Prompt Engineering & Context Mastery

**Duration:** Week 1–2 | **Sessions:** 6 (Sessions 1–6)
**Milestone Project:** AURA v0.1 — CLI-based prompt-powered chatbot with evaluation discipline

### Learning Objectives
By the end of this module, the learner will be able to:
- Write, evaluate and systematically improve prompts for a variety of tasks
- Understand how tokenization affects LLM behavior and cost
- Manage context windows effectively in multi-turn conversations
- Implement structured output formatting and output parsing

---

### Session 1 — How LLMs Actually Work (Whiteboarding Intensive)

**Topics Covered:**
- Transformer architecture conceptually — attention, weights, probability
- What "generation" really means: next-token prediction
- Temperature, top_p, top_k, frequency penalty — intuition and use cases
- The anatomy of a prompt: system, user, assistant turns
- **Whiteboard Exercise:** Draw the prompt → tokenize → model → response pipeline

**Hands-on Lab:**
```
Lab 1.1 — The Token Counter
- Use tiktoken (OpenAI) and Anthropic's token counter
- Send identical prompts to one current OpenAI model and one current Anthropic model
- Compare token counts, response lengths, costs
- Observe how rephrasing changes token usage
- AURA Task: Write the first system prompt for AURA
```

**Tools:** Python, tiktoken, openai SDK, anthropic SDK

---

### Session 2 — Tokenization & Context Window Deep Dive

**Topics Covered:**
- How BPE (Byte Pair Encoding) tokenization works — live demonstration
- Context window limits: compare current OpenAI, Anthropic, and Gemini models
- What happens when context window is exceeded — truncation strategies
- Context compression techniques: summarization, sliding window, chunking
- **Whiteboard Exercise:** Diagram a sliding-window context management strategy

**Hands-on Lab:**
```
Lab 1.2 — Context Window Stress Test
- Build a simple multi-turn chat that tracks token usage per turn
- Implement a "summarize and compress" strategy when approaching limits
- Visualize the context budget in a simple dashboard
- AURA Task: Add context tracking to AURA v0.1's conversation loop
```

**Tools:** Python, tiktoken, LiteLLM for unified token tracking

---

### Session 3 — Prompt Engineering Fundamentals

**Topics Covered:**
- Zero-shot, few-shot, one-shot prompting — when to use each
- Reasoning-oriented prompting: asking for concise rationales, plans, assumptions, and verifiable steps
- Why not to rely on hidden chain-of-thought: prefer structured outputs, scratchpad-free explanations, and tests
- Role prompting and persona assignment
- Instruction following vs. instruction tuning
- Negative prompting: what NOT to say
- **Whiteboard Exercise:** Build a prompt taxonomy tree

**Hands-on Lab:**
```
Lab 1.3 — Prompt Engineering Workshop
- Solve 5 tasks using only prompt engineering (no code changes)
  1. Structured JSON extraction from unstructured text
  2. Multi-step math reasoning with concise visible rationale and verification
  3. Code explanation with step-by-step breakdown
  4. Tone transformation (formal ↔ casual)
  5. Multi-class classification with confidence scores
- AURA Task: Make AURA respond as a research assistant persona
```

---

### Session 4 — Advanced Prompt Patterns & Context Engineering

**Topics Covered:**
- System prompt architecture: layering rules, personas, tool definitions
- Context injection patterns: dynamic context, retrieved context, user context
- Prompt chaining: breaking complex tasks into sequential prompts
- ReAct prompting pattern (Reason + Act) — foundation for agents
- **Whiteboard Exercise:** Design a prompt chain for a multi-step research task

**Hands-on Lab:**
```
Lab 1.4 — Prompt Chaining Pipeline
- Build a 3-step prompt chain:
  Step 1: Extract key topics from a document
  Step 2: Research each topic (simulated)
  Step 3: Synthesize into a structured report
- Each step's output feeds the next step's context
- AURA Task: Add a "research pipeline" mode to AURA v0.1
```

---

### Session 5 — Prompt Evaluation Methodology

**Topics Covered:**
- Why prompt evaluation matters: consistency, reliability, regression
- Evaluation dimensions: accuracy, relevance, coherence, groundedness, toxicity
- Manual evaluation rubrics and scoring guides
- LLM-as-a-Judge pattern — using GPT/Claude to evaluate GPT/Claude
- Prompt regression testing: catching degradations when prompts change
- **Whiteboard Exercise:** Design an evaluation scorecard for a chatbot

**Hands-on Lab:**
```
Lab 1.5 — Build an LLM Evaluator
- Create a dataset of 20 prompt-response pairs (golden dataset)
- Write an LLM-as-a-Judge prompt that scores responses on:
  1. Correctness (0–10)
  2. Relevance (0–10)
  3. Conciseness (0–10)
- Run evaluations and compare two different system prompts
- AURA Task: Create AURA's first evaluation dataset (20 QA pairs)
```

**Tools:** Python, openai/anthropic SDK, pandas, JSON

---

### Session 6 — Module 1 Milestone: AURA v0.1

**Milestone Project Build Day**

```
🎯 AURA v0.1 — CLI Research Chatbot

Requirements:
✅ CLI-based multi-turn conversation with AURA
✅ Custom system prompt with research assistant persona
✅ Context window tracking (displays token usage per turn)
✅ Context compression when approaching 80% of limit
✅ Prompt chaining: can run a 3-step research pipeline
✅ Basic LLM-as-a-Judge evaluation on 20 golden examples
✅ Support for both OpenAI and Anthropic backends (configurable)
✅ Cost estimation display after each response
✅ Prompt regression test can be re-run after prompt changes

Deliverables:
- Working CLI application (Python)
- System prompt documentation
- Evaluation dataset (20 examples) with scores
- README with design decisions
- Portfolio note: what changed after evaluation and why

Whiteboard Review: Draw AURA's architecture. Walk through context flow.
```

---

## MODULE 2: AI Integration, Model APIs & Error Handling

**Duration:** Week 3–4 | **Sessions:** 6 (Sessions 7–12)
**Milestone Project:** AURA v0.2 — Robust multi-model AI integration layer

### Learning Objectives
- Build production-grade API integration with OpenAI and Anthropic
- Handle streaming, errors, retries, and timeouts gracefully
- Implement caching strategies to reduce cost and latency
- Understand structured output, function calling, and tool use primitives
- Expose AURA through a small FastAPI service with OpenAPI documentation
- Apply early security practices: secrets, logging hygiene, PII handling, and tool permissions

---

### Session 7 — Production-Grade API Integration

**Topics Covered:**
- OpenAI API deep dive: Responses API, structured outputs, tool calling, streaming
- Assistants API as legacy/optional context, not the primary implementation path
- Anthropic API deep dive: Messages API, streaming, tool use
- API key management and security best practices (env vars, secrets managers)
- Rate limits, quotas, and API tier management
- LiteLLM as a unified proxy layer for multi-provider support
- **Whiteboard Exercise:** Design a multi-provider AI integration layer

**Hands-on Lab:**
```
Lab 2.1 — Unified AI Client
- Build an AIClient class that wraps both OpenAI and Anthropic
- Support model switching via config (not code changes)
- Implement automatic fallback: if primary fails → use secondary
- Log request/response metadata without storing secrets, raw PII, or full sensitive prompts
- AURA Task: Replace AURA's hardcoded client with AIClient
```

---

### Session 8 — Streaming, Async & Concurrency

**Topics Covered:**
- Server-Sent Events (SSE) and streaming token delivery
- Why streaming matters for UX and perceived performance
- Async Python with asyncio — concurrent API calls
- Parallel prompt execution vs. sequential chaining
- **Whiteboard Exercise:** Streaming pipeline vs. batch processing trade-offs

**Hands-on Lab:**
```
Lab 2.2 — Streaming & Async Integration
- Add streaming support to AIClient (display tokens as they arrive)
- Convert AURA's conversation loop to async
- Run 3 parallel sub-queries and merge results
- Measure wall-clock time: streaming vs. awaiting full response
- AURA Task: Add streaming output to AURA's research pipeline
```

---

### Session 9 — LLM Error Handling, Retries & Timeouts

**Topics Covered:**
- Categories of LLM errors: rate limits, context exceeded, content policy, server errors
- Exponential backoff retry strategies
- Circuit breaker pattern for LLM calls
- Graceful degradation: what to return when the LLM fails
- Timeout strategies and budget enforcement
- Secure error handling: do not leak stack traces, secrets, tenant data, or raw provider payloads
- **Whiteboard Exercise:** Error state machine for LLM API calls

**Hands-on Lab:**
```
Lab 2.3 — Resilient LLM Client
- Add retry with exponential backoff to AIClient (tenacity library)
- Implement circuit breaker: stop retrying after 3 failures in 60s
- Add per-request timeout (max 30s per call)
- Handle content policy violations gracefully (log + fallback message)
- Simulate errors and verify recovery behavior
- Add structured security logs with redaction
- AURA Task: Make AURA's API layer production-resilient
```

**Tools:** tenacity, asyncio, aiohttp

---

### Session 10 — Structured Outputs & Function/Tool Calling

**Topics Covered:**
- Pydantic models for enforcing structured LLM output
- OpenAI structured outputs (JSON mode, json_schema enforcement)
- Anthropic tool use: defining tools, parsing tool calls, returning results
- Function calling as the foundation for agentic behavior
- Output parsing and validation pipelines
- Tool permissioning: allowlists, argument validation, timeouts, and human approval boundaries
- **Whiteboard Exercise:** Tool call lifecycle — define → invoke → return → re-prompt

**Hands-on Lab:**
```
Lab 2.4 — Tool-Calling Integration
- Define 3 tools: web_search (mock), calculator, date_lookup
- Implement the full tool-use loop:
  1. Model decides to call a tool
  2. Parse the tool call from response
  3. Execute the tool
  4. Return result back to model
  5. Model provides final answer
- Use Pydantic for strict output validation
- Add validation and timeout limits for every tool
- AURA Task: Give AURA 3 tools: web_search, doc_lookup (mock), summarizer
```

---

### Integrated Mini-Lab — FastAPI Product Wrapper

This mini-lab should be spread across Sessions 10-12 so the session count remains unchanged.

**Topics Covered:**
- Why AI builders need API delivery, not only notebooks and CLIs
- FastAPI route design for chat, retrieval, evaluation, and health checks
- Request/response schemas with Pydantic
- OpenAPI / Swagger as a portfolio and integration artifact
- Basic authentication options: API key now, OAuth/JWT later

**Hands-on Lab:**
```
Mini-Lab — AURA API Surface
- Add FastAPI endpoints:
  - POST /chat
  - POST /research
  - GET /health
  - GET /metrics/basic
- Generate OpenAPI docs automatically
- Add request IDs and structured logging
- AURA Task: AURA can now be demonstrated through Swagger UI, not only CLI
```

---

### Session 11 — Caching Strategies for LLMs

**Topics Covered:**
- Why caching matters: cost reduction and latency improvement, with realistic measurement
- Semantic caching vs. exact-match caching
- Prompt prefix caching (OpenAI and Anthropic native support)
- Cache-aside pattern with Redis for LLM responses
- Cache invalidation strategies: TTL, content hash, version tags
- **Whiteboard Exercise:** Cache decision tree — what to cache and for how long

**Hands-on Lab:**
```
Lab 2.5 — Semantic Cache Layer
- Install and configure Redis (local Docker container)
- Implement exact-match cache (hash prompt → cache response)
- Implement semantic cache using embedding similarity (cosine > 0.95 = cache hit)
- Measure: latency reduction and cost savings with cache enabled
- Test cache invalidation with TTL
- AURA Task: Add a semantic cache layer to AURA
```

**Tools:** Redis, sentence-transformers, hashlib

---

### Session 12 — Module 2 Milestone: AURA v0.2

```
🎯 AURA v0.2 — Production-Grade AI Integration Layer

New Capabilities Added:
✅ Unified AIClient supporting OpenAI + Anthropic (configurable)
✅ Automatic provider fallback on failure
✅ Streaming output in the CLI
✅ Async concurrent sub-queries
✅ Retry logic with exponential backoff + circuit breaker
✅ Graceful error handling with user-friendly messages
✅ 3 integrated tools: web_search (mock), doc_lookup, summarizer
✅ Full tool-calling loop with Pydantic output validation
✅ Semantic cache layer (Redis-backed)
✅ Real-time cost + latency display per response
✅ FastAPI wrapper with Swagger/OpenAPI documentation
✅ Security baseline: secret management, redacted logs, request IDs, tool allowlists

Deliverables:
- Updated AURA codebase with test suite
- Error handling runbook (document all error states)
- Cache hit-rate report (run 50 queries, measure savings)
- OpenAPI screenshot or exported schema
- Security checklist covering secrets, logs, PII, and tool permissions

Whiteboard Review: Draw the complete request lifecycle including caching,
error handling, tool calls, and fallback paths.
```

---

# MONTH 2 — RAG, Frameworks, Evaluation & Observability

> **Theme:** Give your agent knowledge. Make it measurable. Make it debuggable.

---

## MODULE 3: RAG — Retrieval-Augmented Generation

**Duration:** Week 5–7 | **Sessions:** 9 (Sessions 13–21)
**Milestone Project:** AURA v0.3 — Knowledge-grounded research assistant

### Learning Objectives
- Build a full RAG pipeline from document ingestion to retrieval to generation
- Understand embeddings, vector databases, and similarity search
- Implement chunking strategies and their impact on retrieval quality
- Build hybrid retrieval combining dense and sparse search
- Evaluate retrieval and answer quality with repeatable test sets
- Defend RAG applications against prompt injection and unsafe retrieved content

---

### Session 13 — Embeddings: The Foundation of Semantic Search

**Topics Covered:**
- What embeddings are: dense vector representations of meaning
- How embedding models work: encoder-only transformers (BERT family)
- Embedding model comparison: OpenAI text-embedding-3-large, Cohere, BGE, E5
- Cosine similarity, dot product, and Euclidean distance
- Embedding dimensions, storage costs, and performance trade-offs
- **Whiteboard Exercise:** Visualize semantic similarity in 2D embedding space

**Hands-on Lab:**
```
Lab 3.1 — Embedding Explorer
- Generate embeddings for 100 sentences using 3 different models
- Compute cosine similarity between sentence pairs
- Visualize embedding clusters using UMAP (2D projection)
- Compare embedding quality on a retrieval benchmark (50 queries)
- AURA Task: Set up the embedding pipeline for AURA's knowledge base
```

**Tools:** openai embeddings, sentence-transformers, numpy, umap-learn, matplotlib

---

### Session 14 — Vector Databases: Architecture & Selection

**Topics Covered:**
- Vector DB landscape: Pinecone, Weaviate, Chroma, Qdrant, pgvector, FAISS
- HNSW (Hierarchical Navigable Small World) index — how ANN search works
- Filtering: metadata filtering alongside vector search
- Scalability considerations: index size, query throughput, update frequency
- Managed vs. self-hosted trade-offs
- Required-path decision: Qdrant as the primary implementation; others as comparison context
- **Whiteboard Exercise:** Design a vector DB schema for a multi-tenant knowledge base

**Hands-on Lab:**
```
Lab 3.2 — Vector DB Setup & Benchmarking
- Set up ChromaDB (local) and Qdrant (Docker)
- Index 1,000 documents with metadata (source, date, category)
- Run similarity searches with metadata filters
- Benchmark: query latency at p50/p95/p99
- Compare FAISS (in-memory) vs. ChromaDB vs. Qdrant for 10K vectors
- AURA Task: Connect AURA to a Qdrant vector store
```

**Tools:** ChromaDB, Qdrant, FAISS, Docker

---

### Session 15 — Document Processing & Chunking Strategies

**Topics Covered:**
- Document loaders: PDF, DOCX, HTML, CSV, Markdown, web scraping
- Chunking strategies:
  - Fixed-size chunking
  - Recursive character text splitting
  - Semantic chunking (split on meaning shifts)
  - Hierarchical chunking (parent-child relationships)
- Chunk size vs. retrieval precision trade-offs
- Metadata extraction and enrichment during ingestion
- **Whiteboard Exercise:** Compare chunking strategies on a long research paper

**Hands-on Lab:**
```
Lab 3.3 — Ingestion Pipeline
- Build a document ingestion pipeline supporting PDF, DOCX, HTML, MD
- Implement all 4 chunking strategies
- Evaluate each strategy on the same 10 retrieval queries
- Add metadata: source URL, document title, page number, creation date
- AURA Task: Build AURA's knowledge base ingestion pipeline
  (ingest 50 tech blog posts + 10 research papers)
```

**Tools:** LangChain document loaders, pypdf, python-docx, BeautifulSoup

---

### Session 16 — Building the Retrieval Pipeline

**Topics Covered:**
- Naive RAG: query → embed → retrieve → inject → generate
- Query expansion and query rewriting for better retrieval
- Re-ranking with cross-encoders (Cohere Rerank, BGE reranker)
- Hybrid search: combining BM25 (sparse) + vector (dense) search
- Reciprocal Rank Fusion (RRF) for combining ranked lists
- **Whiteboard Exercise:** Draw a production retrieval pipeline with re-ranking

**Hands-on Lab:**
```
Lab 3.4 — Advanced Retrieval Pipeline
- Implement naive RAG baseline
- Add query expansion: generate 3 query variants, merge results
- Add BM25 sparse retrieval (rank_bm25 library)
- Implement hybrid search with RRF fusion
- Add Cohere Rerank (or cross-encoder) as a re-ranking stage
- Measure MRR@10 and Recall@10 for each configuration
- AURA Task: Upgrade AURA with hybrid retrieval + re-ranking
```

**Tools:** rank_bm25, sentence-transformers cross-encoder, Cohere API

---

### Session 17 — Advanced RAG Patterns

**Topics Covered:**
- Self-Query RAG: LLM generates a structured query with filters
- Multi-Query RAG: generate multiple sub-queries in parallel
- Contextual compression: compress retrieved chunks before injection
- RAG Fusion: merge ranked lists from multiple retrieval strategies
- RAPTOR: recursive abstractive processing for hierarchical retrieval (advanced optional)
- Parent-document retrieval: retrieve child chunks, inject parent context
- **Whiteboard Exercise:** When to use which advanced RAG pattern (decision tree)

**Hands-on Lab:**
```
Lab 3.5 — Advanced RAG Patterns
- Implement Self-Query RAG with metadata filtering
- Implement Multi-Query RAG with parallel retrieval
- Implement Contextual Compression Retriever
- Compare all 3 + baseline on a 30-question test set
- Mark RAPTOR and knowledge graph integrations as stretch tasks only
- AURA Task: Enable Self-Query and Multi-Query modes in AURA
```

---

### Session 18 — RAG Evaluation Framework

**Topics Covered:**
- RAG evaluation dimensions:
  - **Retrieval:** Context Precision, Context Recall, MRR
  - **Generation:** Faithfulness, Answer Relevancy, Answer Correctness
- RAGAS framework: automated RAG evaluation
- Building test sets: reference-based and reference-free evaluation
- Using LLM judges for faithfulness scoring
- Cost of evaluation: when to run full eval vs. spot checks
- **Whiteboard Exercise:** Design an end-to-end RAG evaluation pipeline

**Hands-on Lab:**
```
Lab 3.6 — RAG Evaluation with RAGAS
- Install and configure RAGAS
- Create a test dataset: 30 questions + ground-truth answers + relevant contexts
- Evaluate AURA's RAG pipeline on:
  - Context Precision
  - Context Recall
  - Faithfulness
  - Answer Relevancy
- Generate an evaluation report and identify weakest dimensions
- AURA Task: Build AURA's automated evaluation pipeline
```

**Tools:** RAGAS, pandas, matplotlib

---

### Session 19 — Indexing Strategies & Knowledge Base Maintenance

**Topics Covered:**
- Incremental indexing: adding new documents without re-indexing everything
- Deduplication strategies in vector databases
- Handling document updates and deletions (vector DB versioning)
- Multi-modal RAG: indexing images alongside text (CLIP, GPT-4V)
- Knowledge graph integration: combining RAG with structured knowledge
- **Whiteboard Exercise:** Knowledge base lifecycle management diagram

**Hands-on Lab:**
```
Lab 3.7 — Production Knowledge Base Management
- Implement incremental ingestion (only embed new/changed documents)
- Add document deduplication (content hash comparison)
- Implement soft deletes with versioned documents
- Schedule a nightly re-indexing job (APScheduler)
- AURA Task: Set up AURA's knowledge base maintenance pipeline
```

---

### Session 20 — Integrating RAG into the Agent Loop

**Topics Covered:**
- RAG as a tool: giving the agent a retrieval function to call on demand
- Adaptive RAG: decide whether to retrieve based on query type
- Corrective RAG (CRAG): grade retrieved documents, web-search if poor quality
- Grounded generation: citation injection and source attribution
- RAG security: prompt injection inside retrieved documents, untrusted URLs, source allowlists
- Citation quality: every important factual claim should trace back to source chunks
- **Whiteboard Exercise:** Adaptive RAG decision flow diagram

**Hands-on Lab:**
```
Lab 3.8 — Agentic RAG
- Implement a "retrieve or not" decision gate (LLM grades query type)
- Implement CRAG: if all retrieved docs score < 0.5 relevance, fall back to web search
- Add citation injection: every factual claim annotated with source
- Add retrieved-context safety checks before passing content to the model
- AURA Task: AURA now retrieves from knowledge base as a tool call,
  with CRAG fallback to web search
```

---

### Session 21 — Module 3 Milestone: AURA v0.3

```
🎯 AURA v0.3 — Knowledge-Grounded Research Assistant

New Capabilities Added:
✅ Document ingestion pipeline (PDF, DOCX, HTML, MD)
✅ Semantic chunking with metadata enrichment
✅ Qdrant vector store integration
✅ Hybrid retrieval: BM25 + dense search with RRF fusion
✅ Cross-encoder re-ranking stage
✅ Self-Query and Multi-Query retrieval modes
✅ Contextual Compression Retriever
✅ CRAG: corrective retrieval with web-search fallback
✅ Citation injection in generated responses
✅ Automated RAGAS evaluation pipeline
✅ Incremental indexing + nightly re-index scheduler
✅ RAG security checks for untrusted retrieved content and source allowlists

Deliverables:
- Ingested knowledge base: 50+ documents
- RAGAS evaluation report (baseline vs. advanced pipeline)
- Architecture diagram of the full RAG pipeline
- Retrieval failure analysis: 5 examples where the system gave weak or missing evidence

Whiteboard Review: Walk through a complete query lifecycle from
user question → retrieval → re-ranking → generation → citation.
```

---

## MODULE 4: LangChain, LangGraph & Observability

**Duration:** Week 8–9 | **Sessions:** 6 (Sessions 22–27)
**Milestone Project:** AURA v0.4 — Graph-based agent with full observability

### Learning Objectives
- Build stateful, cyclical agent workflows using LangGraph
- Implement observability with Langfuse as the required path and LangSmith as optional comparison
- Evaluate and compare agent trajectories
- Understand agent memory patterns within a graph
- Add CI-friendly evaluation gates for prompts, RAG, and agent workflows

---

### Session 22 — LangChain Core Concepts

**Topics Covered:**
- LangChain primitives: Runnables, Chains, LLMs, ChatModels, OutputParsers
- LCEL (LangChain Expression Language): pipe operator composition
- Prompt templates: ChatPromptTemplate, MessagesPlaceholder
- Memory in LangChain/LangGraph: current memory patterns, checkpointing, summaries, and state
- LangChain vs. direct SDK usage — when to use each
- **Whiteboard Exercise:** Map out a RAG chain using LCEL

**Hands-on Lab:**
```
Lab 4.1 — LCEL-Powered Pipelines
- Rebuild AURA's RAG pipeline using LCEL
- Build a retrieval chain: prompt | retriever | llm | output_parser
- Add summarized conversation state or checkpoint-backed memory to AURA
- Compare LCEL composition vs. manual pipeline
- AURA Task: Migrate AURA's core to LCEL-based architecture
```

---

### Session 23 — LangGraph: Stateful Agent Graphs

**Topics Covered:**
- Why graphs for agents: cycles, branching, human-in-the-loop
- LangGraph primitives: StateGraph, Nodes, Edges, Conditional Edges
- Defining agent state: TypedDict, Annotated reducers
- The ReAct agent as a graph: think → act → observe → loop
- Interrupts and checkpointing: pausing execution for human approval
- **Whiteboard Exercise:** Draw AURA's agent flow as a LangGraph state machine

**Hands-on Lab:**
```
Lab 4.2 — Building a ReAct Agent in LangGraph
- Implement a ReAct loop in LangGraph:
  - "agent" node: LLM decides next action
  - "tools" node: executes the chosen tool
  - Conditional edge: "should_continue" → agent or END
- Add state: track conversation history, tool call history, retrieved docs
- Add a "human_approval" interrupt before executing sensitive tools
- AURA Task: Rebuild AURA as a LangGraph agent
```

**Tools:** langgraph, langchain-core

---

### Session 24 — Complex Graph Topologies

**Topics Covered:**
- Parallel node execution in LangGraph
- Subgraphs: composing smaller graphs into larger workflows
- Map-reduce patterns: fan-out tasks then aggregate results
- Error handling within graphs: retry nodes, fallback branches
- Long-running task management with background execution
- **Whiteboard Exercise:** Design a multi-step research workflow as a graph

**Hands-on Lab:**
```
Lab 4.3 — Advanced Graph Topologies
- Implement a parallel research graph:
  - Fan out: 3 parallel "topic researcher" subgraphs
  - Fan in: "synthesizer" node aggregates all 3 results
- Add error handling: if a subgraph fails, use cached result
- Add a map-reduce summarization pipeline
- AURA Task: Add a parallel multi-topic research mode to AURA
```

---

### Session 25 — Agent Tracing & Evaluation

**Topics Covered:**
- Trace anatomy: project → trace → run → span
- Automatic tracing of LangChain and LangGraph applications
- Evaluation datasets: creating, versioning, and reusing examples
- Custom evaluators and LLM-graded evals
- LangSmith as optional hosted comparison; Langfuse remains the required stack
- **Whiteboard Exercise:** Tracing hierarchy — project → trace → run → span

**Hands-on Lab:**
```
Lab 4.4 — Trace-Based Evaluation
- Run 20 queries and inspect full traces
- Create a dataset from 15 real traces
- Run a configured evaluator: faithfulness + relevance scoring
- Compare two AURA versions (v0.2 RAG vs. v0.3 CRAG) side-by-side
- Optional: repeat the same experiment in LangSmith
- AURA Task: Add repeatable trace-based evaluation to AURA
```

**Tools:** Langfuse, LangSmith (optional hosted comparison), langchain tracing SDK

---

### Session 26 — Langfuse: Required Observability, Latency & Cost Tracking

**Topics Covered:**
- Langfuse vs. LangSmith: feature comparison and use cases
- Langfuse Cloud or self-hosted Langfuse with Docker Compose
- Tracing spans: LLM calls, retrieval, tool use, complete traces
- Latency tracking: p50, p95, p99 per span type
- Cost tracking: per-model, per-user, per-feature cost attribution
- Prompt versioning, release labels, and A/B testing in Langfuse
- Production evaluation sampling: what to score, how often, and how to control cost
- **Whiteboard Exercise:** Design a monitoring dashboard for an agent system

**Hands-on Lab:**
```
Lab 4.5 — Langfuse Observability
- Use Langfuse Cloud or deploy Langfuse locally with Docker Compose
- Instrument AURA with Langfuse SDK (trace all LLM + retrieval spans)
- Build a monitoring dashboard showing:
  - Average latency per query type (p50/p95/p99)
  - Daily cost breakdown by model
  - Cache hit rate
  - Retrieval quality over time
- Set up a latency alert: notify if p95 > 5s
- AURA Task: Switch AURA's production observability to Langfuse
```

**Tools:** Langfuse Cloud or self-hosted Docker, langfuse SDK, Docker Compose

---

### Session 27 — Module 4 Milestone: AURA v0.4

```
🎯 AURA v0.4 — Evaluated, Observable Graph-Based Agent

New Capabilities Added:
✅ LangGraph-based ReAct agent architecture
✅ Parallel research subgraphs (fan-out + fan-in)
✅ Human-in-the-loop approval interrupts
✅ LCEL-based chain composition
✅ ConversationSummaryBufferMemory
✅ Langfuse full tracing + evaluation datasets
✅ Optional LangSmith comparison report
✅ Latency tracking (p50/p95/p99 by span)
✅ Cost attribution per model per query type
✅ Automated evaluation pipeline with scoring
✅ CI-friendly eval gate for a small regression dataset

Deliverables:
- Working LangGraph agent with trace visualization
- Langfuse dashboard screenshots showing cost + latency metrics
- Evaluation dataset (20 examples) with scores
- Comparison report: AURA v0.2 vs. v0.4 performance
- CI eval-gate output showing pass/fail criteria

Whiteboard Review: Walk through a complete trace — every node,
edge decision, tool call, retrieval span, and LLM call in sequence.
```

---

# MONTH 3 — Agent Workflows, Memory, LLMOps & Cloud Deployment

> **Theme:** Go to production. Scale up. Handle the real world.

---

## MODULE 5: Role-Based Agent Workflows & Agent Memory

**Duration:** Week 10–11 | **Sessions:** 6 (Sessions 28–33)
**Milestone Project:** AURA v0.5 — Role-based agent workflow with persistent memory and guardrails

### Learning Objectives
- Design and implement role-based agent workflows with specialized responsibilities
- Build persistent and episodic memory systems for agents
- Implement agent communication and orchestration patterns
- Handle task delegation, review loops, and human approval boundaries
- Know when multi-agent systems add value and when a simpler graph is better

---

### Session 28 — Agent Memory Architecture

**Topics Covered:**
- The 4 memory types:
  - **Semantic memory:** facts about the world (RAG knowledge base)
  - **Episodic memory:** records of past interactions (conversation history)
  - **Procedural memory:** how to do things (system prompts, tools)
  - **Working memory:** current context window
- Memory storage backends: Redis, PostgreSQL, Vector DB, file system
- Memory retrieval: when and what to retrieve automatically
- Memory compression and forgetting strategies
- **Whiteboard Exercise:** Design AURA's complete memory architecture

**Hands-on Lab:**
```
Lab 5.1 — Multi-Tier Memory System
- Implement episodic memory: store and retrieve past conversation summaries
- Implement semantic memory: persist user preferences and learned facts
- Build a "memory retrieval" step that automatically injects relevant
  memories into each new conversation context
- Add memory management: user can view, edit, delete memories
- AURA Task: Give AURA persistent memory across sessions
```

**Tools:** Redis (episodic), PostgreSQL + pgvector (semantic), SQLAlchemy

---

### Session 29 — Role-Based Agent Design Patterns

**Topics Covered:**
- Why multi-agent: specialization, parallelism, review, and workflow clarity
- When not to use multi-agent: added latency, cost, debugging complexity, and coordination failure
- Multi-agent topologies:
  - **Supervisor-Worker:** orchestrator delegates to specialized agents
  - **Peer-to-Peer:** agents communicate directly
  - **Hierarchical:** nested supervisor structures
  - **Pipeline:** agents pass results sequentially
- Agent specialization: researcher, writer, critic, planner, executor
- Inter-agent communication: message passing, shared state, tool handoffs
- **Whiteboard Exercise:** Design a 3-role research workflow topology

**Hands-on Lab:**
```
Lab 5.2 — Supervisor Role Workflow
- Implement a 3-role system in LangGraph:
  - Supervisor: routes tasks and synthesizes results
  - Researcher: queries web + knowledge base
  - Writer: formats and writes the final output
- Optional stretch role: Analyst interprets tabular or numerical data
- Implement supervisor routing logic (LLM-based routing)
- Add inter-agent message passing via shared graph state
- AURA Task: Transform AURA into a role-based research workflow
```

---

### Session 30 — Agent Coordination & Conflict Resolution

**Topics Covered:**
- Consensus patterns: voting, averaging, judge-based selection
- Debate pattern: agents argue for their answer, judge selects best
- Critic agent: reviews output and requests revisions
- Task decomposition: breaking complex tasks into parallel sub-tasks
- Deadlock detection and prevention in agent graphs
- Cost and latency controls for review loops
- **Whiteboard Exercise:** Debate pattern flow — propose → critique → revise → select

**Hands-on Lab:**
```
Lab 5.3 — Critic and Review Loops
- Add a Critic agent to AURA's pipeline that reviews Researcher output
- Add a Judge step that scores answer quality, citations, and uncertainty
- Optional stretch: implement a one-round debate between Researcher and Critic
- Implement task decomposition: for multi-part questions, spawn parallel
  sub-agents and aggregate results
- AURA Task: AURA now validates high-value research outputs through Critic + Judge
```

---

### Session 31 — Agent Execution Environments & Tool Ecosystems

**Topics Covered:**
- Code execution agents: sandboxed Python execution (E2B, Modal, CodeInterpreter)
- Browser automation agents: Playwright, Selenium for web interaction
- File system agents: read/write/create documents
- API integration agents: REST, GraphQL, webhooks
- Tool registry pattern: dynamically discovering and loading tools
- **Whiteboard Exercise:** Agent capability matrix — which agent needs which tool

**Hands-on Lab:**
```
Lab 5.4 — Extended Tool Ecosystem
- Add E2B sandboxed code execution to AURA's Analyst agent
- Add Playwright-based web scraping tool for Researcher agent
- Add a file creation tool for Writer agent (generate .md/.docx reports)
- Build a tool registry: tools self-register with descriptions
- AURA Task: Full tool ecosystem — AURA can write and run code,
  browse the web, and produce downloadable reports
```

**Tools:** E2B Python SDK, playwright-python, tool registry pattern

---

### Session 32 — Human-in-the-Loop & Agent Guardrails

**Topics Covered:**
- When to require human approval: irreversible actions, high-stakes decisions
- LangGraph interrupt patterns: sync and async human approval
- Guardrails: input validation, output filtering, content moderation
- Policy self-check patterns: self-evaluation before responding
- Hallucination detection: identifying and flagging uncertain claims
- Budget guardrails: hard stop on token/cost limits per session
- **Whiteboard Exercise:** Guardrail pipeline — where to check, what to block

**Hands-on Lab:**
```
Lab 5.5 — Guardrails & Safety Layer
- Add input guardrails: block prompt injection, PII, harmful queries
- Add output guardrails: detect and flag hallucinations (low-confidence claims)
- Implement a policy self-check before final response
- Add hard budget guardrail: stop if session exceeds $0.50 or 100K tokens
- Implement human approval for: web requests, code execution, report generation
- AURA Task: Deploy AURA's full safety and guardrail layer
```

**Tools:** Guardrails AI or NeMo Guardrails, LangGraph interrupt

---

### Session 33 — Module 5 Milestone: AURA v0.5

```
🎯 AURA v0.5 — Role-Based Agent Workflow with Memory

New Capabilities Added:
✅ Multi-tier persistent memory (episodic + semantic)
✅ Memory retrieval injected automatically into context
✅ 3-role workflow: Supervisor, Researcher, Writer
✅ Optional Analyst role for code/data execution
✅ Critic + Judge review loop for high-value outputs
✅ Task decomposition with parallel sub-agent spawning
✅ Sandboxed code execution (E2B)
✅ Web browsing capability (Playwright)
✅ Downloadable report generation (.md, .docx)
✅ Tool registry with dynamic tool loading
✅ Full guardrail layer: input + output + budget
✅ Human-in-the-loop approval for sensitive actions
✅ Policy self-check before responses

Deliverables:
- Demo: AURA answers a complex research question using the role-based workflow
- Memory demo: AURA recalls user preferences from a previous session
- Guardrail test report: 10 adversarial inputs, all blocked correctly
- Cost/latency report comparing simple RAG vs. role-based workflow

Whiteboard Review: Draw the complete multi-agent coordination diagram —
state flow, agent responsibilities, tool assignments, memory layers.
```

---

## MODULE 6: LLMOps, AgentOps & Cloud Infrastructure

**Duration:** Week 12–13 | **Sessions:** 6 (Sessions 34–39)
**Milestone Project:** AURA v1.0 — Production-deployed, monitored system

### Learning Objectives
- Deploy AI agents to one cloud platform: AWS or Azure
- Understand managed inference first, with self-hosted model serving as an advanced option
- Implement CI/CD pipelines for AI systems
- Build production-grade monitoring and alerting
- Build runbooks for eval failures, cost spikes, latency regressions, and provider outages

---

### Session 34 — Cloud AI Platforms & Model Hosting

**Topics Covered:**
- Cloud AI platform overview:
  - **AWS:** Bedrock, SageMaker, AgentCore as optional platform context
  - **Azure:** Azure AI Foundry, Azure OpenAI, Prompt Flow
  - **GCP:** Vertex AI Agent Engine
- Model hosting options:
  - Managed inference (Bedrock, Azure OpenAI) — no infra management
  - Dedicated endpoints (SageMaker endpoints, Azure ML)
  - Self-hosted on GPU VMs (vLLM, TGI, Ollama) — advanced optional path
  - Serverless inference (AWS Lambda + Bedrock, Azure Functions)
- Latency vs. cost vs. control trade-off matrix
- Required-path decision: choose AWS or Azure for implementation, not both
- **Whiteboard Exercise:** Choose the right deployment architecture for 3 use cases

**Hands-on Lab:**
```
Lab 6.1 — Cloud Platform Integration
- Choose one primary cloud path: AWS Bedrock or Azure OpenAI
- Integrate AURA with the selected managed provider
- Optional: deploy a small open-source model locally via Ollama
- Benchmark: latency + cost for the same query across local dev vs. cloud
- AURA Task: Make AURA configurable for local dev and one production provider
```

**Tools:** boto3 or azure-openai, ollama (optional), Docker

---

### Session 35 — Inference Optimization & Optional Self-Hosted Serving

**Topics Covered:**
- Required path: model selection, routing, prompt caching, batching trade-offs, and latency budgets
- Open-source model serving: vLLM, Text Generation Inference (TGI), Ollama (advanced)
- Model quantization: FP16, INT8, INT4 — quality vs. speed vs. memory (advanced)
- KV cache: what it is and why it matters for multi-turn agents
- Speculative decoding and draft models for latency reduction
- GPU memory estimation: how to size your deployment (advanced)
- **Whiteboard Exercise:** Serving architecture — load balancer → vLLM cluster → monitoring

**Hands-on Lab:**
```
Lab 6.2 — Inference Cost and Latency Optimization
- Build a model-routing policy: cheap model for simple tasks, stronger model for complex tasks
- Add prompt caching and response streaming measurements
- Benchmark 50 test queries by cost, latency, quality, and fallback rate
- Optional advanced lab: point AURA's AIClient at an Ollama or vLLM endpoint
- AURA Task: Add routing and latency/cost optimization to AURA
```

**Tools:** provider SDKs, Docker, Ollama optional, vLLM optional

---

### Session 36 — Containerization & CI/CD for AI Systems

**Topics Covered:**
- Dockerizing a LangGraph agent application
- Docker Compose for multi-service stacks: API + vector DB + Redis + Langfuse
- GitHub Actions CI pipeline: lint → test → build → push → deploy
- Environment configuration management: .env, secrets, config maps
- Testing AI systems: unit tests for chains, integration tests for tools
- Eval gates in CI: small regression set for prompts, RAG, and agent traces
- Blue-green deployment and canary releases for AI agents
- **Whiteboard Exercise:** CI/CD pipeline diagram for an AI agent system

**Hands-on Lab:**
```
Lab 6.3 — Dockerize & CI/CD Pipeline
- Write Dockerfile for AURA (multi-stage build)
- Create docker-compose.yml: AURA API + Qdrant + Redis + Langfuse
- Write GitHub Actions workflow:
  Step 1: Run pytest (unit + integration tests)
  Step 2: Run a small eval regression suite
  Step 3: Build Docker image
  Step 4: Push to GitHub Container Registry
  Step 5: Deploy to cloud (simulated or real)
- Write 10 integration tests for AURA's key agent behaviors
- AURA Task: Full containerization + CI/CD pipeline
```

**Tools:** Docker, Docker Compose, GitHub Actions, pytest

---

### Session 37 — Cloud Deployment: AWS or Azure

**Topics Covered:**
- Deploying containerized agents on:
  - **AWS ECS/Fargate** — serverless container orchestration
  - **Azure Container Apps** — serverless containers on Azure
  - **AWS AgentCore** — purpose-built agent runtime (preview)
- API Gateway setup: REST API in front of the agent service
- Authentication: API keys, JWT, OAuth2 for agent endpoints
- Auto-scaling: scale based on request queue depth and latency
- Cost optimization: reserved capacity vs. on-demand for inference
- Production privacy basics: network boundaries, secrets, logs, and access control
- **Whiteboard Exercise:** Production deployment architecture diagram for the selected cloud

**Hands-on Lab:**
```
Lab 6.4 — Deploy AURA to One Cloud
- Deploy AURA to AWS ECS Fargate or Azure Container Apps:
  - Configure task definition / container app spec
  - Set up Application Load Balancer
  - Configure auto-scaling (min 1, max 5 instances)
  - Set up API Gateway with API key authentication
- Test deployed endpoint with curl and Python client
- AURA Task: AURA v1.0 is live at an authenticated API endpoint
```

**Tools:** AWS CLI, AWS CDK or Terraform (basic), or Azure CLI

---

### Session 38 — Production Monitoring, Alerting & LLMOps

**Topics Covered:**
- LLMOps / AgentOps vs. traditional MLOps — what's different
- LLMOps / AgentOps terminology: evals, traces, costs, prompt versions, tool failures, and incident response
- Key agent metrics to monitor:
  - Latency: time-to-first-token, total response time
  - Quality: automated LLM-judge scores in production
  - Cost: per-request, per-user, per-day spend
  - Reliability: error rate, retry rate, fallback rate
  - Business: task completion rate, user satisfaction
- Drift detection for RAG: retrieval quality over time
- Alerting: PagerDuty/Slack alerts for SLA breaches
- Production evaluation: shadow mode, A/B testing, champion-challenger
- Runbooks: what to do when quality drops, cost spikes, latency regresses, or a provider fails
- **Whiteboard Exercise:** Design AURA's SLOs and alerting runbook

**Hands-on Lab:**
```
Lab 6.5 — Production Monitoring Dashboard
- Configure Langfuse production alerts:
  - Alert if p95 latency > 8 seconds
  - Alert if daily cost exceeds $20
  - Alert if error rate > 5% in 5-minute window
- Implement production LLM judge: score every 10th response automatically
- Build a Grafana dashboard (or use Langfuse):
  - Real-time latency chart
  - Cost-per-hour trend
  - Retrieval quality score trend
  - Error rate gauge
- Simulate a degraded scenario and verify alerting fires
- AURA Task: AURA v1.0 has full production monitoring
```

**Tools:** Langfuse (hosted or self-hosted), Grafana + Prometheus (optional)

---

### Session 39 — Module 6 Milestone: AURA v1.0

```
🎯 AURA v1.0 — Production-Deployed, Monitored AI Agent System

New Capabilities Added:
✅ Local development provider + one selected production cloud provider
✅ Fully containerized with Docker + Docker Compose
✅ CI/CD pipeline: GitHub Actions → test → eval gate → build → deploy
✅ Deployed to AWS ECS Fargate (or Azure Container Apps)
✅ Authenticated API endpoint with API key or JWT authentication
✅ Auto-scaling based on load
✅ Real-time monitoring: latency, cost, quality, error rate
✅ Automated production evaluation (every 10th response scored)
✅ Alerting configured for SLA breaches
✅ Deployment runbook documented
✅ Incident runbooks for eval failures, cost spikes, latency regressions, and provider outages

Deliverables:
- Live deployed AURA endpoint or documented local production simulation URL
- Monitoring dashboard screenshot
- CI/CD pipeline logs showing green build
- Cost analysis: estimated monthly cost at 100 daily users

Whiteboard Review: Full production architecture — from user request
through API Gateway, ECS, agent graph, tools, RAG, cache, to monitoring.
```

---

# CAPSTONE PROJECT

**Duration:** Week 13 final session + independent completion
**Format:** Team or individual (presenter chooses scope)

---

## 🎓 AURA Enterprise — Production Portfolio Solution

The capstone is a 5-day sprint to package AURA v1.0 into one polished, scenario-specific AI product. The goal is not to add every possible feature; the goal is to demonstrate production judgment, measurable quality, secure design, and a clear career-ready portfolio artifact.

### Capstone Requirements

The learner chooses ONE of the following enterprise scenarios to deploy AURA into:

**Option A: Enterprise Knowledge Management System**
> AURA deployed as an internal knowledge assistant for a company — indexes internal documents, answers employee questions, generates reports, and stores curated feedback.

**Option B: Autonomous Research & Competitive Intelligence Agent**
> AURA deployed as a market intelligence tool — monitors news sources, builds a knowledge base, generates competitive analyses, and proactively alerts on significant market events.

**Option C: AI-Powered Software Engineering Assistant**
> AURA deployed as a developer productivity tool — understands a codebase, answers architecture questions, drafts code changes, reviews PRs, and monitors code quality with human approval for write actions.

---

### Capstone Minimum Requirements

Regardless of scenario, the final project must demonstrate the following required scope. Stretch items can be added only after the required scope is complete.

```
FOUNDATION (from Modules 1-2):
✅ Custom system prompt with documented prompt engineering decisions
✅ Production-grade API integration with error handling + fallback
✅ Exact-match or semantic caching with measurable hit rate
✅ Token budget management with context compression
✅ FastAPI service with OpenAPI documentation

RAG PIPELINE (from Module 3):
✅ Ingestion pipeline for scenario-specific document types
✅ Vector retrieval with metadata filters
✅ Hybrid retrieval or re-ranking
✅ Evaluation report on retrieval and answer quality
✅ Source citations and fallback strategy documented

AGENT ARCHITECTURE (from Modules 4-5):
✅ LangGraph-based agent with documented state machine
✅ Minimum 2 specialized roles or workflow nodes
✅ Persistent memory for user preferences or prior sessions
✅ Tool ecosystem with minimum 3 tools
✅ Guardrail layer with documented safety tests
✅ Human approval for at least one sensitive action

PRODUCTION (from Module 6):
✅ Dockerized with CI/CD pipeline
✅ Deployed to one cloud provider or a clearly documented local production simulation
✅ Full observability: latency + cost + quality dashboards
✅ Alerting or explicit SLO checks configured and tested
✅ Automated evaluation on a sample of production-like traces

DOCUMENTATION:
✅ Architecture Decision Record (ADR) document
✅ System architecture diagram
✅ API documentation (OpenAPI/Swagger)
✅ Runbook: deploy, scale, monitor, debug, rollback
✅ Cost model: estimated cost at 3 usage tiers
✅ Demo video or scripted live demo path
```

**Optional Stretch Scope**
- Multi-agent debate pattern
- vLLM or Ollama self-hosted model endpoint
- Multi-cloud deployment
- RAPTOR, knowledge graph integration, or multimodal RAG
- Slack, Teams, GitHub, or Jira integration

---

### Capstone Deliverables & Presentation

**Presentation Format (60 minutes):**

| Time | Segment |
|------|---------|
| 0–5 min | Problem statement and solution overview |
| 5–15 min | Live demo of the deployed system |
| 15–25 min | Architecture walkthrough (whiteboard) |
| 25–35 min | Evaluation results: RAG quality, agent quality, latency |
| 35–45 min | Monitoring dashboard walkthrough |
| 45–55 min | Design decisions and trade-offs |
| 55–60 min | Q&A and lessons learned |

---

# Program Summary & Skill Map

## Complete Skills Coverage Matrix

| Skill Area | Module | Depth |
|------------|--------|-------|
| Prompt Engineering | M1 | ⭐⭐⭐⭐⭐ |
| Prompt Evaluation | M1, M4 | ⭐⭐⭐⭐⭐ |
| Tokenization & Context Windows | M1 | ⭐⭐⭐⭐ |
| OpenAI API Integration | M2 | ⭐⭐⭐⭐⭐ |
| Anthropic API Integration | M2 | ⭐⭐⭐⭐⭐ |
| LLM Error Handling | M2 | ⭐⭐⭐⭐⭐ |
| Caching (Exact + Semantic) | M2 | ⭐⭐⭐⭐ |
| Embeddings | M3 | ⭐⭐⭐⭐⭐ |
| Vector Databases | M3 | ⭐⭐⭐⭐⭐ |
| RAG Pipeline | M3 | ⭐⭐⭐⭐⭐ |
| RAG Evaluation (RAGAS) | M3 | ⭐⭐⭐⭐ |
| LangChain / LCEL | M4 | ⭐⭐⭐⭐ |
| LangGraph | M4, M5 | ⭐⭐⭐⭐⭐ |
| LangSmith | M4 | ⭐⭐ optional comparison |
| Langfuse | M4 | ⭐⭐⭐⭐ required path |
| Latency & Cost Tracking | M4, M6 | ⭐⭐⭐⭐⭐ |
| Agent Memory | M5 | ⭐⭐⭐⭐⭐ |
| Role-Based Agent Workflows | M5 | ⭐⭐⭐⭐ |
| Agent Guardrails | M5 | ⭐⭐⭐⭐ |
| Human-in-the-Loop | M4, M5 | ⭐⭐⭐⭐ |
| Model Serving (vLLM/Ollama) | M6 | ⭐⭐⭐ |
| Model Quantization | M6 | ⭐⭐⭐ |
| Cloud Deployment (AWS/Azure) | M6 | ⭐⭐⭐⭐ |
| AWS AgentCore / AI Foundry | M6 | ⭐⭐ optional platform context |
| LLMOps / AgentOps / CI-CD for AI | M6 | ⭐⭐⭐⭐ |
| Production Monitoring | M6 | ⭐⭐⭐⭐⭐ |

---

## AURA Evolution Summary

```
AURA v0.1  ─── CLI chatbot with prompt engineering + basic evaluation
    │
    ▼
AURA v0.2  ─── Multi-model API layer + error handling + caching + tool calls
    │
    ▼
AURA v0.3  ─── RAG pipeline + hybrid retrieval + CRAG + citations + RAGAS
    │
    ▼
AURA v0.4  ─── LangGraph agent + parallel subgraphs + Langfuse + optional LangSmith
    │
    ▼
AURA v0.5  ─── Role-based workflow + persistent memory + guardrails + sandboxed tools
    │
    ▼
AURA v1.0  ─── Cloud deployed + CI/CD + auto-scaling + production monitoring
    │
    ▼
AURA Enterprise ─── Capstone: focused production portfolio project with complete docs
```

---

## Recommended Tools & Stack Reference

| Category | Tools |
|----------|-------|
| **LLM APIs** | OpenAI current flagship/efficient models, Anthropic current Sonnet/Haiku models, selected cloud provider model endpoint |
| **Unified LLM Layer** | LiteLLM, Ollama |
| **Agent Frameworks** | LangChain, LangGraph |
| **Observability** | Langfuse (primary), LangSmith (optional), Grafana |
| **Vector DBs** | Qdrant (primary), ChromaDB (dev), FAISS (in-memory) |
| **Embedding Models** | text-embedding-3-large, BGE-M3, E5-large |
| **Caching** | Redis (semantic + session cache) |
| **RAG Evaluation** | RAGAS |
| **Model Serving** | vLLM, Ollama, TGI |
| **Cloud** | AWS (ECS, Bedrock; AgentCore as optional context), Azure (Container Apps, AI Foundry) |
| **Containerization** | Docker, Docker Compose |
| **CI/CD** | GitHub Actions |
| **Databases** | PostgreSQL + pgvector, Redis |
| **Testing** | pytest, pytest-asyncio |
| **Languages** | Python 3.11+, TypeScript (optional) |

Before each cohort begins, verify current model names, pricing, context windows, deprecations, and SDK syntax from the official provider documentation. AI platform details change quickly, so the curriculum should teach provider-agnostic patterns while using current examples in class.

---

## Pre-Program Setup Checklist

Before Session 1, complete the following:

```bash
# Python environment
python -m venv aura-env
pip install openai anthropic langchain langgraph langchain-community
pip install langsmith langfuse ragas chromadb qdrant-client
pip install redis sentence-transformers rank-bm25 tiktoken
pip install fastapi uvicorn pytest pytest-asyncio tenacity pydantic pydantic-settings python-dotenv httpx ruff pypdf python-docx beautifulsoup4

# Docker (for Redis, Qdrant, Langfuse)
docker pull redis:7-alpine
docker pull qdrant/qdrant
# For Langfuse, use Langfuse Cloud or follow the current Docker Compose docs

# API Keys to obtain before starting:
# ✅ OpenAI API key (platform.openai.com)
# ✅ Anthropic API key (console.anthropic.com)
# ✅ Langfuse API keys (cloud or local)
# ✅ LangSmith API key (optional hosted comparison)
# ✅ Cohere API key (cohere.com) — for reranking
# ✅ AWS account or Azure account for the selected deployment path
```

---

## Recommended Learning Resources (By Module)

**Module 1 — Prompt Engineering**
- Anthropic's Prompt Engineering Guide: docs.anthropic.com/en/docs/build-with-claude/prompt-engineering
- OpenAI Prompt Engineering Guide: platform.openai.com/docs/guides/prompt-engineering
- DeepLearning.AI: "ChatGPT Prompt Engineering for Developers"

**Module 2 — API Integration**
- OpenAI Function Calling Docs
- Anthropic Tool Use Docs
- LiteLLM Documentation: docs.litellm.ai

**Module 3 — RAG**
- LangChain RAG Documentation
- RAGAS Documentation: docs.ragas.io
- Paper: "Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks" (Lewis et al.)
- Paper: "Self-RAG" and "Corrective RAG"

**Module 4 — LangGraph & Observability**
- LangGraph Documentation: langchain-ai.github.io/langgraph
- LangSmith Documentation
- Langfuse Documentation: langfuse.com/docs

**Module 5 — Role-Based Agents**
- Paper: "CAMEL: Communicative Agents for 'Mind' Exploration"
- Paper: "AutoGen: Enabling Next-Gen LLM Applications via Multi-Agent Conversation"
- LangGraph Multi-Agent Architectures Guide

**Module 6 — LLMOps, AgentOps & Cloud**
- AWS Bedrock User Guide
- Azure AI Foundry Documentation
- "Designing Machine Learning Systems" by Chip Huyen

---

*Program designed for software engineers with Python proficiency. No prior ML experience required.*
*Estimated completion: 13 weeks at the defined schedule (117 contact hours + ~50 hours independent work)*
