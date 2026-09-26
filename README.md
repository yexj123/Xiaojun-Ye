# Hi there, I'm Xiaojun Ye

### Academic Profile
- **Master's Student in AI & Robotics** at the **University of Padua** (Unipd).
- **B.Sc. in Ingegneria Informatica (Computer Engineering)** from the University of Padua.

### Tech Stack & Tools
- **Languages:** Python
- **AI / Agents:** LangGraph, OpenAI API, DeepSeek, PyTorch, Scikit-learn, NumPy, Pandas
- **Backend:** FastAPI, SQLite (FTS5 / BM25), Server-Sent Events, Jinja2 + htmx
- **Testing & Eval:** pytest, DeepEval, paired A/B evaluation harnesses
- **Tools:** Git, uv, conda, Claude Code, MCP

### Competitions
- **HackerRank Orchestrate (Sept 2026):** Ranked **191 / 3,062**, built an intent & purchase
  prediction pipeline combining deterministic rule-based triage with a single-layer LLM
  decision architecture.

### Main Project

**[deep-research](https://github.com/yexj123/deep-research)** — a self-hosted deep research
agent. Give it a research question: it plans subtopics, searches arXiv for each in parallel,
and writes a literature review that **cites only papers it actually retrieved**.
Python · LangGraph · FastAPI · SQLite. No build step, no `node_modules`.

Built to be **measured, not demoed**:

- Recursive decomposition, deeper search and full-text retrieval were each implemented,
  evaluated against a frozen question set, and found **not** to improve review quality — so
  the agent that ships is *cheaper than its first design*, with no measured quality cost.
- The local BM25 corpus did pay, in cost rather than quality: **65 arXiv requests became 1
  and wall clock fell 65%**, with every quality metric unchanged.
- 140 committed evaluation recordings regenerate every table in the findings with **no API
  key**, so the claims are reproducible by anyone who clones it.
- Grounded citations, streamed token-by-token over SSE, resumable runs via LangGraph
  checkpoints, and a multi-turn follow-up mode. ~975 tests.

### Learning & Coursework
- **[AI Portfolio Monorepo](https://github.com/yexj123/ai-portfolio-monorepo):** agentic
  systems and fine-tuning projects built while learning:
  - **[LLM Chatbot Fine-Tuning](https://github.com/yexj123/ai-portfolio-monorepo/tree/main/projects/chatbot-finetuned):** chatbot
fine-tuning based on the Hugging Face NLP Course.
  - **[Simple Research
Assistant](https://github.com/yexj123/ai-portfolio-monorepo/tree/main/projects/simple_research_assistant):** progressive
exploration of agentic design patterns with the OpenAI API.
  - **[Research Assistant with
MCP](https://github.com/yexj123/ai-portfolio-monorepo/tree/main/projects/simple_research_assistant_mcp):** agentic workflows
integrated with FastMCP, stdio servers, and hosted remote tools.
- **[Thesis Assistant with LangGraph](https://github.com/yexj123/lang_graph_assistant):** earlier
  LangGraph agent for thesis writing.
- **[PyTorch exercises](https://github.com/yexj123/torch)** · **[Scikit-learn
exercises](https://github.com/yexj123/ml-exercises):** comparative studies.

### How to reach me
- **Email:** xiaojun.ye1312@gmail.com
