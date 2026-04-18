Hi, I'm Cynthia 👋🏽
Backend engineer focused on building reliable, AI-powered systems — from secure REST APIs to RAG pipelines and real-time streaming.

Portfolio: cynthia-kalu-o-portfolio.netlify.app Open to: Backend roles (junior & internship) · Remote · On-site · Visa sponsorship welcome


🚀 Projects
🏥 MediBook API — Healthcare Appointment System
A production-grade booking API where clinics manage doctors and slots, patients book appointments, and the system handles real-world concurrency and communication.

What makes it interesting:

Atomic slot-locking at the database transaction level — prevents double-booking entirely, even under concurrent load
AI urgency classification (GPT-4o-mini) recommends appointments by severity: low, medium, or high
Celery + Redis background tasks handle email confirmations, cancellations, and 24h reminders without blocking booking responses
15s OpenAI timeout + 2-retry logic with latency logging — resilient AI integration, not naive

Stack: FastAPI · PostgreSQL · SQLAlchemy 2.0 async · OpenAI · Celery · Redis · Google OAuth · Docker · Render

🔗 Live API · 📁 Repository


📚 ScholarIQ AI — RAG-Powered Academic Writing API
An API where hallucinated citations are structurally impossible — not filtered, not detected after the fact, but architecturally prevented.

What makes it interesting:

Full RAG pipeline built from scratch: PDF ingestion → chunking → OpenAI embedding → pgvector storage → similarity search → grounded generation
GPT-4o-mini only sees retrieved chunks from the user's own uploaded documents — no access to external knowledge during generation
Vector similarity search with pgvector (cosine distance) surfaces the most relevant document sections for any query
Three-table schema: users, documents, document_chunks — each chunk stores its embedding as a vector column
Returns generated text alongside source citations: document name, page number, and excerpt

Stack: FastAPI · PostgreSQL · pgvector · SQLAlchemy 2.0 async · OpenAI text-embedding-3-small · GPT-4o-mini · PyMuPDF · SlowAPI · Docker · Render · Neon

🔗 Live API · 📁 Repository


🧠 Cerebro API — Real-Time Socratic AI Conversation
An API where the AI doesn't generate ideas for you — it challenges yours. Built with SSE streaming and persistent conversation history.

What makes it interesting:

Token-by-token SSE streaming — users see the AI response building in real time, not a block of text after a wait
The AI is explicitly prompted to question, challenge, and redirect — not just respond
Full conversation history persisted in PostgreSQL; users can return to any thread and continue
Fully async architecture: SQLAlchemy 2.0 async + asyncpg throughout

Stack: FastAPI · PostgreSQL · SQLAlchemy 2.0 async · OpenAI GPT-4o-mini · SSE Streaming · JWT · Docker · Render

🔗 Live API · 📁 Repository


🛠️ Tech Stack
Languages: Python 3.11+

Frameworks: FastAPI · SQLAlchemy 2.0 async · Pydantic v2 · Alembic

Databases: PostgreSQL · pgvector · Neon · Redis

AI / ML: OpenAI GPT-4o-mini · text-embedding-3-small · RAG pipelines · SSE streaming

Auth: JWT · Google OAuth 2.0 · API key auth

Infrastructure: Docker · Render · Celery · SlowAPI · python-json-logger

Tools: Git · GitHub · VS Code · Postman


📌 Current Focus
Building and iterating on production-grade backend systems
Deepening knowledge of RAG architecture and vector search
Engaging with senior engineers publicly and shipping feedback within 24 hours


📫 Connect
💼 LinkedIn
🐦 X / Twitter
🌐 Portfolio
