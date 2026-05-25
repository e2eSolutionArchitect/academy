# 🤖 AI Builder Career Transformation Program
---

> **Program Duration:** 3 Months | **Schedule:** 3 Days/Week × 3 Hours/Day = **~108 Hours Total**
> **Format:** Hands-on Coding + Whiteboarding Sessions
> **Target Learner:** Software Engineers transitioning to AI/Agent development
> **Goal:** Design, Build, Deploy, Monitor & Debug production-standard Agentic solutions

---

## Program Overview

```
┌─────────────────────────────────────────────────────────────────────┐
│                    LEARNING JOURNEY MAP                              │
│                                                                     │
│  Month 1                Month 2               Month 3              │
│  ┌──────────┐           ┌──────────┐          ┌──────────┐         │
│  │ MODULE 1 │──────────▶│ MODULE 3 │─────────▶│ MODULE 5 │         │
│  │Foundations│          │  RAG &   │          │  Multi-  │         │
│  │& Prompts  │          │ Vectors  │          │  Agent   │         │
│  └──────────┘           └──────────┘          └──────────┘         │
│  ┌──────────┐           ┌──────────┐          ┌──────────┐         │
│  │ MODULE 2 │──────────▶│ MODULE 4 │─────────▶│ MODULE 6 │         │
│  │AI Integr.│          │Frameworks│          │ MLOps &  │         │
│  │& Tokens  │          │& Evals   │          │  Cloud   │         │
│  └──────────┘           └──────────┘          └──────────┘         │
│                                                      │              │
│                                                      ▼              │
│                                               ┌──────────┐         │
│                                               │ CAPSTONE │         │
│                                               │ PROJECT  │         │
│                                               └──────────┘         │
└─────────────────────────────────────────────────────────────────────┘
```

---

## 🏗️ The Evolving Project: **AURA** — *Autonomous Unified Research Assistant*

Throughout the entire program, you will build a single evolving project that grows in capability and production-readiness with each module. By the end, AURA will be a fully deployed, monitored, multi-agent enterprise knowledge assistant.

| Module | AURA Evolution Stage |
|--------|---------------------|
| Module 1 | AURA v0.1 — Basic prompt-powered chatbot |
| Module 2 | AURA v0.2 — Multi-model, token-aware assistant |
| Module 3 | AURA v0.3 — RAG-enabled knowledge assistant |
| Module 4 | AURA v0.4 — Evaluated, tool-using agent |
| Module 5 | AURA v0.5 — Multi-agent memory system |
| Module 6 | AURA v1.0 — Production-deployed, monitored system |
| Capstone | AURA Enterprise — Full agentic solution |

---

## 📅 Session Schedule & Structure

Each 3-hour session follows this rhythm:

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
**Milestone Project:** AURA v0.1 — CLI-based prompt-powered chatbot

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
- Send identical prompts to GPT-4o and Claude 3.5 Sonnet
- Compare token counts, response lengths, costs
- Observe how rephrasing changes token usage
- AURA Task: Write the first system prompt for AURA
```

**Tools:** Python, tiktoken, openai SDK, anthropic SDK

---

### Session 2 — Tokenization & Context Window Deep Dive

**Topics Covered:**
- How BPE (Byte Pair Encoding) tokenization works — live demonstration
- Context window limits: GPT-4o (128K), Claude 3.5 (200K), Gemini (1M)
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
- Chain-of-Thought (CoT) and Tree-of-Thought (ToT) prompting
- Role prompting and persona assignment
- Instruction following vs. instruction tuning
- Negative prompting: what NOT to say
- **Whiteboard Exercise:** Build a prompt taxonomy tree

**Hands-on Lab:**
```
Lab 1.3 — Prompt Engineering Workshop
- Solve 5 tasks using only prompt engineering (no code changes)
  1. Structured JSON extraction from unstructured text
  2. Multi-step math reasoning with CoT
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

Deliverables:
- Working CLI application (Python)
- System prompt documentation
- Evaluation dataset (20 examples) with scores
- README with design decisions

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

---

### Session 7 — Production-Grade API Integration

**Topics Covered:**
- OpenAI API deep dive: Chat Completions, Responses API, Assistants API
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
- Log all API calls with request/response metadata
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
- **Whiteboard Exercise:** Error state machine for LLM API calls

**Hands-on Lab:**
```
Lab 2.3 — Resilient LLM Client
- Add retry with exponential backoff to AIClient (tenacity library)
- Implement circuit breaker: stop retrying after 3 failures in 60s
- Add per-request timeout (max 30s per call)
- Handle content policy violations gracefully (log + fallback message)
- Simulate errors and verify recovery behavior
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
- AURA Task: Give AURA 3 tools: web_search, doc_lookup (mock), summarizer
```

---

### Session 11 — Caching Strategies for LLMs

**Topics Covered:**
- Why caching matters: cost reduction (up to 90%) and latency improvement
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

Deliverables:
- Updated AURA codebase with test suite
- Error handling runbook (document all error states)
- Cache hit-rate report (run 50 queries, measure savings)

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

**Tools:** LangChain document loaders, PyPDF2, python-docx, BeautifulSoup

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
- RAPTOR: recursive abstractive processing for hierarchical retrieval
- Parent-document retrieval: retrieve child chunks, inject parent context
- **Whiteboard Exercise:** When to use which advanced RAG pattern (decision tree)

**Hands-on Lab:**
```
Lab 3.5 — Advanced RAG Patterns
- Implement Self-Query RAG with metadata filtering
- Implement Multi-Query RAG with parallel retrieval
- Implement Contextual Compression Retriever
- Compare all 3 + baseline on a 30-question test set
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
- **Whiteboard Exercise:** Adaptive RAG decision flow diagram

**Hands-on Lab:**
```
Lab 3.8 — Agentic RAG
- Implement a "retrieve or not" decision gate (LLM grades query type)
- Implement CRAG: if all retrieved docs score < 0.5 relevance, fall back to web search
- Add citation injection: every factual claim annotated with source
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

Deliverables:
- Ingested knowledge base: 50+ documents
- RAGAS evaluation report (baseline vs. advanced pipeline)
- Architecture diagram of the full RAG pipeline

Whiteboard Review: Walk through a complete query lifecycle from
user question → retrieval → re-ranking → generation → citation.
```

---

## MODULE 4: LangChain, LangGraph & Observability

**Duration:** Week 8–9 | **Sessions:** 6 (Sessions 22–27)
**Milestone Project:** AURA v0.4 — Graph-based agent with full observability

### Learning Objectives
- Build stateful, cyclical agent workflows using LangGraph
- Implement observability with LangSmith and Langfuse
- Evaluate and compare agent trajectories
- Understand agent memory patterns within a graph

---

### Session 22 — LangChain Core Concepts

**Topics Covered:**
- LangChain primitives: Runnables, Chains, LLMs, ChatModels, OutputParsers
- LCEL (LangChain Expression Language): pipe operator composition
- Prompt templates: ChatPromptTemplate, MessagesPlaceholder
- Memory in LangChain: ConversationBufferMemory, SummaryMemory
- LangChain vs. direct SDK usage — when to use each
- **Whiteboard Exercise:** Map out a RAG chain using LCEL

**Hands-on Lab:**
```
Lab 4.1 — LCEL-Powered Pipelines
- Rebuild AURA's RAG pipeline using LCEL
- Build a retrieval chain: prompt | retriever | llm | output_parser
- Add ConversationSummaryBufferMemory to AURA
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

### Session 25 — LangSmith: Tracing & Evaluation

**Topics Covered:**
- LangSmith architecture: traces, runs, feedback, datasets
- Automatic tracing of LangChain and LangGraph applications
- Evaluating runs in LangSmith: custom evaluators, LLM-graded evals
- Dataset management: creating and versioning evaluation datasets
- A/B testing prompts in LangSmith Playground
- **Whiteboard Exercise:** Tracing hierarchy — project → trace → run → span

**Hands-on Lab:**
```
Lab 4.4 — LangSmith Observability
- Connect AURA to LangSmith (LANGCHAIN_TRACING_V2=true)
- Run 20 queries and inspect full traces in the LangSmith UI
- Create a dataset from 15 real traces
- Run a configured evaluator: faithfulness + relevance scoring
- Compare two AURA versions (v0.2 RAG vs. v0.3 CRAG) side-by-side
- AURA Task: Enable LangSmith tracing as AURA's primary observability layer
```

**Tools:** LangSmith (hosted), langchain tracing SDK

---

### Session 26 — Langfuse: Open-Source Observability & Latency/Cost Tracking

**Topics Covered:**
- Langfuse vs. LangSmith: feature comparison and use cases
- Self-hosted Langfuse with Docker Compose
- Tracing spans: LLM calls, retrieval, tool use, complete traces
- Latency tracking: p50, p95, p99 per span type
- Cost tracking: per-model, per-user, per-feature cost attribution
- Prompt versioning and A/B testing in Langfuse
- **Whiteboard Exercise:** Design a monitoring dashboard for an agent system

**Hands-on Lab:**
```
Lab 4.5 — Langfuse Self-Hosted Observability
- Deploy Langfuse locally with Docker Compose
- Instrument AURA with Langfuse SDK (trace all LLM + retrieval spans)
- Build a monitoring dashboard showing:
  - Average latency per query type (p50/p95/p99)
  - Daily cost breakdown by model
  - Cache hit rate
  - Retrieval quality over time
- Set up a latency alert: notify if p95 > 5s
- AURA Task: Switch AURA's production observability to Langfuse
```

**Tools:** Langfuse (self-hosted Docker), langfuse SDK, Docker Compose

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
✅ LangSmith full tracing + evaluation datasets
✅ Langfuse self-hosted observability dashboard
✅ Latency tracking (p50/p95/p99 by span)
✅ Cost attribution per model per query type
✅ Automated evaluation pipeline with scoring

Deliverables:
- Working LangGraph agent with trace visualization
- Langfuse dashboard screenshots showing cost + latency metrics
- LangSmith evaluation dataset (20 examples) with scores
- Comparison report: AURA v0.2 vs. v0.4 performance

Whiteboard Review: Walk through a complete trace — every node,
edge decision, tool call, retrieval span, and LLM call in sequence.
```

---

# MONTH 3 — Multi-Agent Systems, Memory, MLOps & Cloud Deployment

> **Theme:** Go to production. Scale up. Handle the real world.

---

## MODULE 5: Multi-Agent Systems & Agent Memory

**Duration:** Week 10–11 | **Sessions:** 6 (Sessions 28–33)
**Milestone Project:** AURA v0.5 — Collaborative multi-agent system with persistent memory

### Learning Objectives
- Design and implement multi-agent systems with specialized agents
- Build persistent and episodic memory systems for agents
- Implement agent communication and orchestration patterns
- Handle agent coordination, conflict resolution, and task delegation

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

### Session 29 — Multi-Agent Design Patterns

**Topics Covered:**
- Why multi-agent: specialization, parallelism, reliability through redundancy
- Multi-agent topologies:
  - **Supervisor-Worker:** orchestrator delegates to specialized agents
  - **Peer-to-Peer:** agents communicate directly
  - **Hierarchical:** nested supervisor structures
  - **Pipeline:** agents pass results sequentially
- Agent specialization: researcher, writer, critic, planner, executor
- Inter-agent communication: message passing, shared state, tool handoffs
- **Whiteboard Exercise:** Design a 4-agent research team topology

**Hands-on Lab:**
```
Lab 5.2 — Supervisor Multi-Agent System
- Implement a 4-agent system in LangGraph:
  - Supervisor: routes tasks and synthesizes results
  - Researcher: queries web + knowledge base
  - Analyst: interprets and analyzes data
  - Writer: formats and writes the final output
- Implement supervisor routing logic (LLM-based routing)
- Add inter-agent message passing via shared graph state
- AURA Task: Transform AURA into a multi-agent research team
```

---

### Session 30 — Agent Coordination & Conflict Resolution

**Topics Covered:**
- Consensus patterns: voting, averaging, judge-based selection
- Debate pattern: agents argue for their answer, judge selects best
- Critic agent: reviews output and requests revisions
- Task decomposition: breaking complex tasks into parallel sub-tasks
- Deadlock detection and prevention in agent graphs
- **Whiteboard Exercise:** Debate pattern flow — propose → critique → revise → select

**Hands-on Lab:**
```
Lab 5.3 — Debate & Critic Agents
- Add a Critic agent to AURA's pipeline that reviews Researcher output
- Implement a debate round: Researcher defends findings, Critic challenges
- Add a Judge agent that scores each side and selects the best answer
- Implement task decomposition: for multi-part questions, spawn parallel
  sub-agents and aggregate results
- AURA Task: AURA now validates every research output through Critic + Judge
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
- Constitutional AI patterns: self-evaluation before responding
- Hallucination detection: identifying and flagging uncertain claims
- Budget guardrails: hard stop on token/cost limits per session
- **Whiteboard Exercise:** Guardrail pipeline — where to check, what to block

**Hands-on Lab:**
```
Lab 5.5 — Guardrails & Safety Layer
- Add input guardrails: block prompt injection, PII, harmful queries
- Add output guardrails: detect and flag hallucinations (low-confidence claims)
- Implement Constitutional AI self-check before final response
- Add hard budget guardrail: stop if session exceeds $0.50 or 100K tokens
- Implement human approval for: web requests, code execution, report generation
- AURA Task: Deploy AURA's full safety and guardrail layer
```

**Tools:** Guardrails AI or NeMo Guardrails, LangGraph interrupt

---

### Session 33 — Module 5 Milestone: AURA v0.5

```
🎯 AURA v0.5 — Collaborative Multi-Agent System with Memory

New Capabilities Added:
✅ Multi-tier persistent memory (episodic + semantic)
✅ Memory retrieval injected automatically into context
✅ 4-agent team: Supervisor, Researcher, Analyst, Writer
✅ Critic + Judge agents for output validation
✅ Task decomposition with parallel sub-agent spawning
✅ Sandboxed code execution (E2B)
✅ Web browsing capability (Playwright)
✅ Downloadable report generation (.md, .docx)
✅ Tool registry with dynamic tool loading
✅ Full guardrail layer: input + output + budget
✅ Human-in-the-loop approval for sensitive actions
✅ Constitutional AI self-check before responses

Deliverables:
- Demo: AURA answers a complex research question using all 4 agents
- Memory demo: AURA recalls user preferences from a previous session
- Guardrail test report: 10 adversarial inputs, all blocked correctly

Whiteboard Review: Draw the complete multi-agent coordination diagram —
state flow, agent responsibilities, tool assignments, memory layers.
```

---

## MODULE 6: MLOps, Model Deployment & Cloud Infrastructure

**Duration:** Week 12–13 | **Sessions:** 6 (Sessions 34–39)
**Milestone Project:** AURA v1.0 — Production-deployed, monitored system

### Learning Objectives
- Deploy AI agents to cloud infrastructure (AWS, Azure)
- Understand model hosting, inference optimization, and serving
- Implement CI/CD pipelines for AI systems
- Build production-grade monitoring and alerting

---

### Session 34 — Cloud AI Platforms & Model Hosting

**Topics Covered:**
- Cloud AI platform overview:
  - **AWS:** Bedrock, SageMaker, AgentCore
  - **Azure:** Azure AI Foundry, Azure OpenAI, Prompt Flow
  - **GCP:** Vertex AI Agent Engine
- Model hosting options:
  - Managed inference (Bedrock, Azure OpenAI) — no infra management
  - Dedicated endpoints (SageMaker endpoints, Azure ML)
  - Self-hosted on GPU VMs (vLLM, TGI, Ollama)
  - Serverless inference (AWS Lambda + Bedrock, Azure Functions)
- Latency vs. cost vs. control trade-off matrix
- **Whiteboard Exercise:** Choose the right deployment architecture for 3 use cases

**Hands-on Lab:**
```
Lab 6.1 — Cloud Platform Integration
- Integrate AURA with AWS Bedrock (Claude 3.5 via boto3)
- Integrate AURA with Azure OpenAI (GPT-4o via azure-openai SDK)
- Deploy a small open-source model (Llama 3.1 8B) locally via Ollama
- Benchmark: latency + cost for same query across 3 providers
- AURA Task: Make AURA configurable to use any cloud provider
```

**Tools:** boto3, azure-openai, ollama, Docker

---

### Session 35 — Model Serving, Quantization & Inference Optimization

**Topics Covered:**
- Open-source model serving: vLLM, Text Generation Inference (TGI), Ollama
- Model quantization: FP16, INT8, INT4 — quality vs. speed vs. memory
- Batching strategies: static batching, dynamic batching, continuous batching
- KV cache: what it is and why it matters for multi-turn agents
- Speculative decoding and draft models for latency reduction
- GPU memory estimation: how to size your deployment
- **Whiteboard Exercise:** Serving architecture — load balancer → vLLM cluster → monitoring

**Hands-on Lab:**
```
Lab 6.2 — Local Model Serving with vLLM
- Deploy Llama 3.1 8B with vLLM in Docker
- Benchmark: FP16 vs. INT4 (bitsandbytes) on 50 test queries
- Enable continuous batching and measure throughput improvement
- Point AURA's AIClient at vLLM endpoint (OpenAI-compatible API)
- AURA Task: Add self-hosted vLLM as a third provider option in AURA
```

**Tools:** vLLM, Docker, nvidia-docker (or CPU fallback with Ollama)

---

### Session 36 — Containerization & CI/CD for AI Systems

**Topics Covered:**
- Dockerizing a LangGraph agent application
- Docker Compose for multi-service stacks: API + vector DB + Redis + Langfuse
- GitHub Actions CI pipeline: lint → test → build → push → deploy
- Environment configuration management: .env, secrets, config maps
- Testing AI systems: unit tests for chains, integration tests for tools
- Blue-green deployment and canary releases for AI agents
- **Whiteboard Exercise:** CI/CD pipeline diagram for an AI agent system

**Hands-on Lab:**
```
Lab 6.3 — Dockerize & CI/CD Pipeline
- Write Dockerfile for AURA (multi-stage build)
- Create docker-compose.yml: AURA API + Qdrant + Redis + Langfuse
- Write GitHub Actions workflow:
  Step 1: Run pytest (unit + integration tests)
  Step 2: Build Docker image
  Step 3: Push to GitHub Container Registry
  Step 4: Deploy to cloud (simulated)
- Write 10 integration tests for AURA's key agent behaviors
- AURA Task: Full containerization + CI/CD pipeline
```

**Tools:** Docker, Docker Compose, GitHub Actions, pytest

---

### Session 37 — Cloud Deployment: AWS & Azure

**Topics Covered:**
- Deploying containerized agents on:
  - **AWS ECS/Fargate** — serverless container orchestration
  - **Azure Container Apps** — serverless containers on Azure
  - **AWS AgentCore** — purpose-built agent runtime (preview)
- API Gateway setup: REST API in front of the agent service
- Authentication: API keys, JWT, OAuth2 for agent endpoints
- Auto-scaling: scale based on request queue depth and latency
- Cost optimization: reserved capacity vs. on-demand for inference
- **Whiteboard Exercise:** Production deployment architecture diagram (AWS)

**Hands-on Lab:**
```
Lab 6.4 — Deploy AURA to Cloud
- Deploy AURA to AWS ECS Fargate (or Azure Container Apps):
  - Configure task definition / container app spec
  - Set up Application Load Balancer
  - Configure auto-scaling (min 1, max 5 instances)
  - Set up API Gateway with API key authentication
- Test deployed endpoint with curl and Python client
- AURA Task: AURA v1.0 is live at a public API endpoint
```

**Tools:** AWS CLI, AWS CDK or Terraform (basic), or Azure CLI

---

### Session 38 — Production Monitoring, Alerting & MLOps

**Topics Covered:**
- MLOps for agents vs. traditional MLOps — what's different
- Key agent metrics to monitor:
  - Latency: time-to-first-token, total response time
  - Quality: automated LLM-judge scores in production
  - Cost: per-request, per-user, per-day spend
  - Reliability: error rate, retry rate, fallback rate
  - Business: task completion rate, user satisfaction
- Drift detection for RAG: retrieval quality over time
- Alerting: PagerDuty/Slack alerts for SLA breaches
- Production evaluation: shadow mode, A/B testing, champion-challenger
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
✅ Multi-cloud provider support: AWS Bedrock + Azure OpenAI + self-hosted vLLM
✅ Fully containerized with Docker + Docker Compose
✅ CI/CD pipeline: GitHub Actions → test → build → deploy
✅ Deployed to AWS ECS Fargate (or Azure Container Apps)
✅ Public API endpoint with JWT authentication
✅ Auto-scaling based on load
✅ Real-time monitoring: latency, cost, quality, error rate
✅ Automated production evaluation (every 10th response scored)
✅ Alerting configured for SLA breaches
✅ Deployment runbook documented

Deliverables:
- Live deployed AURA endpoint (public URL)
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

## 🎓 AURA Enterprise — Full-Scale Agentic Solution

The capstone is a 5-day sprint to build AURA Enterprise from AURA v1.0 — a fully featured, production-grade agentic solution that showcases every skill developed throughout the program.

### Capstone Requirements

The learner chooses ONE of the following enterprise scenarios to deploy AURA into:

**Option A: Enterprise Knowledge Management System**
> AURA deployed as an internal knowledge assistant for a company — indexes internal documents, answers employee questions, generates reports, and continuously learns from feedback.

**Option B: Autonomous Research & Competitive Intelligence Agent**
> AURA deployed as a market intelligence tool — monitors news sources, builds a knowledge base, generates competitive analyses, and proactively alerts on significant market events.

**Option C: AI-Powered Software Engineering Assistant**
> AURA deployed as a developer productivity tool — understands a codebase, answers architecture questions, generates code, reviews PRs, and monitors code quality over time.

---

### Capstone Minimum Requirements

Regardless of scenario, the final project must demonstrate all of the following:

```
FOUNDATION (from Modules 1-2):
✅ Custom system prompt with documented prompt engineering decisions
✅ Production-grade API integration with error handling + fallback
✅ Semantic caching with measurable hit rate
✅ Token budget management with context compression

RAG PIPELINE (from Module 3):
✅ Ingestion pipeline for scenario-specific document types
✅ Hybrid retrieval with re-ranking
✅ RAGAS evaluation report on retrieval quality
✅ CRAG with fallback strategy documented

AGENT ARCHITECTURE (from Modules 4-5):
✅ LangGraph-based agent with documented state machine
✅ Minimum 3 specialized agents or roles
✅ Persistent multi-tier memory (episodic + semantic)
✅ Tool ecosystem with minimum 4 tools
✅ Guardrail layer with documented safety tests

PRODUCTION (from Module 6):
✅ Dockerized with CI/CD pipeline
✅ Deployed to cloud with public API endpoint
✅ Full observability: latency + cost + quality dashboards
✅ Alerting configured and tested
✅ Automated production evaluation

DOCUMENTATION:
✅ Architecture Decision Record (ADR) document
✅ System architecture diagram
✅ API documentation (OpenAPI/Swagger)
✅ Runbook: deploy, scale, monitor, debug, rollback
✅ Cost model: estimated cost at 3 usage tiers
```

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
| LangSmith | M4 | ⭐⭐⭐⭐ |
| Langfuse | M4 | ⭐⭐⭐⭐ |
| Latency & Cost Tracking | M4, M6 | ⭐⭐⭐⭐⭐ |
| Agent Memory | M5 | ⭐⭐⭐⭐⭐ |
| Multi-Agent Systems | M5 | ⭐⭐⭐⭐⭐ |
| Agent Guardrails | M5 | ⭐⭐⭐⭐ |
| Human-in-the-Loop | M4, M5 | ⭐⭐⭐⭐ |
| Model Serving (vLLM/Ollama) | M6 | ⭐⭐⭐ |
| Model Quantization | M6 | ⭐⭐⭐ |
| Cloud Deployment (AWS/Azure) | M6 | ⭐⭐⭐⭐ |
| AWS AgentCore / AI Foundry | M6 | ⭐⭐⭐ |
| MLOps / CI-CD for AI | M6 | ⭐⭐⭐⭐ |
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
AURA v0.4  ─── LangGraph agent + parallel subgraphs + LangSmith + Langfuse
    │
    ▼
AURA v0.5  ─── Multi-agent team + persistent memory + guardrails + sandboxed tools
    │
    ▼
AURA v1.0  ─── Cloud deployed + CI/CD + auto-scaling + production monitoring
    │
    ▼
AURA Enterprise ─── Capstone: full enterprise deployment with complete docs
```

---

## Recommended Tools & Stack Reference

| Category | Tools |
|----------|-------|
| **LLM APIs** | OpenAI (GPT-4o), Anthropic (Claude 3.5 Sonnet), AWS Bedrock |
| **Unified LLM Layer** | LiteLLM, Ollama |
| **Agent Frameworks** | LangChain, LangGraph |
| **Observability** | LangSmith, Langfuse, Grafana |
| **Vector DBs** | Qdrant (primary), ChromaDB (dev), FAISS (in-memory) |
| **Embedding Models** | text-embedding-3-large, BGE-M3, E5-large |
| **Caching** | Redis (semantic + session cache) |
| **RAG Evaluation** | RAGAS |
| **Model Serving** | vLLM, Ollama, TGI |
| **Cloud** | AWS (ECS, Bedrock, AgentCore), Azure (Container Apps, AI Foundry) |
| **Containerization** | Docker, Docker Compose |
| **CI/CD** | GitHub Actions |
| **Databases** | PostgreSQL + pgvector, Redis |
| **Testing** | pytest, pytest-asyncio |
| **Languages** | Python 3.11+, TypeScript (optional) |

---

## Pre-Program Setup Checklist

Before Session 1, complete the following:

```bash
# Python environment
python -m venv aura-env
pip install openai anthropic langchain langgraph langchain-community
pip install langsmith langfuse ragas chromadb qdrant-client
pip install redis sentence-transformers rank-bm25 tiktoken
pip install fastapi uvicorn pytest tenacity pydantic python-dotenv

# Docker (for Redis, Qdrant, Langfuse)
docker pull redis:7-alpine
docker pull qdrant/qdrant
docker pull langfuse/langfuse

# API Keys to obtain before starting:
# ✅ OpenAI API key (platform.openai.com)
# ✅ Anthropic API key (console.anthropic.com)
# ✅ LangSmith API key (smith.langchain.com)
# ✅ Cohere API key (cohere.com) — for reranking
# ✅ AWS account (free tier) or Azure account (free tier)
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

**Module 5 — Multi-Agent**
- Paper: "CAMEL: Communicative Agents for 'Mind' Exploration"
- Paper: "AutoGen: Enabling Next-Gen LLM Applications via Multi-Agent Conversation"
- LangGraph Multi-Agent Architectures Guide

**Module 6 — MLOps & Cloud**
- AWS Bedrock User Guide
- Azure AI Foundry Documentation
- "Designing Machine Learning Systems" by Chip Huyen

---

*Program designed for software engineers with Python proficiency. No prior ML experience required.*
*Estimated completion: 13 weeks at the defined schedule (108 contact hours + ~50 hours independent work)*
