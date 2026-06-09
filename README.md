# Hi, I'm Himesh Pandey 👋

**Backend Engineer · AI Systems · PES University, Bengaluru (2026)**

I build production-grade backend systems with a focus on **LLM integration and AI pipelines**. My primary work is around multi-agent workflows, real-time voice AI, RAG architectures, and cost-optimized inference systems using Python.

📍 Bengaluru, India · Open to **full-time roles** (Backend / AI Engineering)  
📫 [pandeyhimesh09@gmail.com](mailto:pandeyhimesh09@gmail.com) · [LinkedIn](https://linkedin.com/in/himesh-pandey-66968a213) · [GitHub](https://github.com/Himeshxx04)

---

## 🔥 Featured Project — MCP Artifact Store

> An open-source MCP server for shared artifact storage across multi-agent LLM pipelines — deployed to production.

**The problem:** Every time Agent A hands off to Agent B in a multi-agent pipeline, it dumps the full payload into shared state. 10 agents = 10x redundant context. This bloats token usage and breaks context windows.

**What I built:**
- **Shared artifact storage** via MCP protocol — agents store and retrieve artifacts by ID, reducing inter-agent context payload from **~1.6KB to 12 bytes** per handoff
- **Dual-interface system** — FastAPI HTTP endpoints for a React dashboard + FastMCP tools for LangGraph agents, backed by a single PostgreSQL service layer
- **Access control + audit logging** — per-artifact permissions, TTL enforcement, creator-only deletion with full audit trail
- **Fully deployed** — FastAPI + FastMCP on Render, PostgreSQL on Render managed DB, React dashboard on Vercel

**Stack:** `FastAPI` `FastMCP` `PostgreSQL` `SQLAlchemy` `LangGraph` `React` `Docker`

🔗 [View the repo →](https://github.com/Himeshxx04/mcp-artifact-store) · 🌐 [Live Dashboard →](https://mcp-artifact-store.vercel.app)

---

## 🎙️ Featured Project — AI Persona (Voice + Chat Agent)

> A voice + chat AI representative that answers technical questions from a resume/GitHub corpus and books real interview slots — across browser WebRTC, SSE chat, and Twilio PSTN.

**What makes it different:**
- **"One brain, two channels"** — shared persona package imported in-process by both the FastAPI chat backend and LiveKit voice worker, eliminating HTTP hops
- **Voice latency: 13s → 1.5s** — parallelized FAISS warm-up with call setup, fixed Deepgram WebSocket reconnects caused by VAD CPU starvation
- **Hallucination guard** — code-level check replays the LLM tool loop when booking phrases appear without `book_slot` actually firing
- **End-to-end booking** — Cal.com integration for real interview scheduling across both voice and chat channels

**Stack:** `FastAPI` `LiveKit` `Deepgram` `ElevenLabs` `FAISS` `OpenAI` `Cal.com API`

🔗 [View the repo →](https://github.com/Himeshxx04/himesh-pandey-ai-persona) · 🌐 [Live →](https://himesh-pandey-ai-persona.vercel.app)

---

## 🛠️ Tech Stack

**Languages:** `Python` `JavaScript` `C` `C++`

**Backend & APIs:** `FastAPI` `REST APIs` `Async/Await` `Middleware` `Pydantic` `SQLAlchemy`

**AI & LLM:** `LangChain` `LangGraph` `LangSmith` `MCP` `RAG` `FAISS` `LiveKit` `Prompt Engineering`

**Databases:** `PostgreSQL` `MySQL` `FAISS Vector Search`

**DevOps & Tools:** `Docker` `Git` `LangSmith` `Ollama` `Wireshark`

---

## 📊 Other Projects

| Project | What it does | Stack |
|---------|-------------|-------|
| [RAG Pipeline Optimizer](https://github.com/Himeshxx04/rag-pipeline-optimizer) | Multi-pipeline RAG with LLM judge evaluation, cost-aware optimization, and hallucination guardrails | FastAPI · FAISS · OpenAI · SQLAlchemy · React |
| [Sales Forecasting API](https://github.com/Himeshxx04/sales-forecasting-api) | End-to-end time series forecasting with SARIMA, Prophet, XGBoost, LSTM | FastAPI · Prophet · XGBoost · LSTM |
| [Chatbot Streaming](https://github.com/Himeshxx04/chatbot-streaming) | Real-time streaming chatbot with token-by-token SSE output | FastAPI · LangChain · SSE |
