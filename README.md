<h1 align="center">Marti Soura Vamseekar</h1>

<p align="center">
  <b>AI & Infrastructure Engineer · M.Sc. Data Science (Greenwich, UK) · Azure DP-203</b><br/>
  RAG/LLM pipelines · Event-driven microservices · Cloud data platforms<br/>
  📍 Hyderabad, India &nbsp;·&nbsp; 🇪🇺 EU Blue Card Eligible · Open to relocation across Germany, Netherlands, Ireland, and wider EU
</p>

<p align="center">
  <a href="https://linkedin.com/in/souramarti"><img src="https://img.shields.io/badge/LinkedIn-souramarti-0077B5?style=flat-square&logo=linkedin"/></a>
  <a href="mailto:martisoura@gmail.com"><img src="https://img.shields.io/badge/Email-martisoura@gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white"/></a>
  <img src="https://img.shields.io/badge/Azure-DP--203-0089D6?style=flat-square&logo=microsoftazure&logoColor=white"/>
  <img src="https://img.shields.io/badge/MSc-Data%20Science%20%7C%20Greenwich-4B0082?style=flat-square"/>
  <img src="https://img.shields.io/badge/EU%20Blue%20Card-Eligible-003399?style=flat-square&logo=europeanunion&logoColor=white"/>
</p>

---

## About Me

AI and Infrastructure Engineer with production experience in RAG/LLM pipelines, event-driven microservices, and cloud data platforms. I work across Google Vertex AI, Java/Spring Boot, Python, Azure Data Factory, Databricks, Docker, Kubernetes, and GCP — delivering across fintech AI research, EU compliance analytics, and government-scale geospatial datasets.

I build things with real depth: a production RAG system over 305 annual reports with FAISS + BM25 + cross-encoder reranking, a 6-service restaurant platform with a 5-country EU VAT engine, a workforce intelligence platform proving labour market tightness correlates with gender pay gaps across 20 EU states, and a UK transport equity analysis covering 56.5 million people.

Targeting EU-based **AI Engineer** or **Data Platform Engineer** roles where production system ownership, deployment reliability, and GenAI infrastructure depth matter.

---

## 💼 Work Experience

### Software Development Engineer — [Innosolv Private Limited](https://innosolv.com)
**London, UK (Remote) · Sep 2025 – Present**

*UK-based fintech delivering algorithmic trading, AI-powered equity research, and market intelligence for NSE cash and F&O markets.*

- **End-to-end AI platform delivery** for Bharat Alpha — institutional equity research system serving 10 NSE sectors; Gemini-powered chat enforces 10 Tier-1 screening filters (ROE >15%, ROCE >15%, D/E <0.8, ICR >2.0, FCF >5%) and a 100-point Tier-2 scoring model; SSE streaming with Supabase Auth and Postgres-persisted conversation history; deployed on GCP
- **Production RAG infrastructure** over 305 annual report filings for 52 Nifty 50 companies (FY2020–FY2025); FAISS IndexFlatIP + BM25 lexical retrieval + reciprocal rank fusion + cross-encoder reranking into a unified pipeline; sector-aware routing across 5 verticals; SSE-streamed responses with inline source citations
- **Algorithmic trading engine** (Java 17, Spring Boot, MongoDB) with AsyncOrderProcessor (CompletableFuture) for non-blocking dispatch and Bucket4j rate limiter at 10 req/s; derivatives suite covers Iron Condor P&L (max-profit filter >2%), multi-leg spread margin engine, basket order aggregator, and participant-wise open interest tracker

`Google Vertex AI` `Gemini` `FAISS` `BM25` `Java 17` `Spring Boot` `GCP` `MongoDB` `RAG` `SSE`

---

## 🚀 Key Projects

### 📊 [WorkforceGuard AI](https://github.com/SVamseekar/workforceguardai) · [Live →](https://workforceguard-ai.vercel.app)
**EU Pay Transparency & Workforce Intelligence Platform · Jan 2024 – Present**

Proved that labour market tightness and gender pay gaps are positively correlated (r ≈ +0.41) across 20 EU member states — grounding EU Pay Transparency Directive 2023/970/EU compliance analysis.

- 36 dbt models across 4 mart layers · DuckDB serverless warehouse · FastAPI backend · React 18 frontend
- GitHub Actions CI/CD deploying in parallel to GCP and Vercel · ingests Eurostat LFS, JVS, SES across 11 NACE sectors · 4 composite workforce indices (HPI, LR, ERS, TR)
- 7 ML models on 32,769 samples — Random Forest: 94.7% accuracy, AUC 0.855, 99.5% recall
- SHA-256 hash-chained SQLite audit log · evidence-bounded Gemini analyst meeting EU Pay Transparency Directive audit requirements

`dbt` `DuckDB` `FastAPI` `React` `scikit-learn` `Gemini` `GitHub Actions` `GCP` `Vercel` `EU Compliance`

---

### 🍽️ [Masova Platform](https://github.com/SVamseekar/masova-platform)
**Cloud-Native Restaurant Management System · Feb 2023 – Present**

- 6 Spring Boot 3 / Java 21 microservices on GCP Cloud Run · 3 durable RabbitMQ topic exchanges · 11-state order state machine with dual-write MongoDB + PostgreSQL · Spring Cloud Gateway with JWT auth and per-route rate limits
- **5-country EU VAT engine** with fiscal signers for Germany (TSE), France (NF525), Belgium (FDM), Italy (RT), Hungary (NTCA)
- 2 WebSocket endpoints (STOMP/SockJS) targeting <100ms state-change delivery · Redis caching · PIN lookup optimised 200ms → 5ms (97.5%)
- Containerised ADK 1.25 / Gemini 2.0 Flash agent · MaSoVaDriverApp (React Native 0.83) with native Android background GPS · 3 notification channels (Brevo, Twilio, Firebase) through GDPR-compliant consent workflows
- Offline queue buffering 1,000 actions with 30-second sync on reconnect

`Spring Boot 3` `Java 21` `GCP Cloud Run` `RabbitMQ` `Spring Cloud Gateway` `MongoDB` `PostgreSQL` `Redis` `Google ADK` `React Native` `GDPR`

---

### 🚌 [Aequitas](https://github.com/SVamseekar/aequitas)
**UK Bus Transport Policy Intelligence Platform · Oct 2021 – Present**

M.Sc. dissertation extended into a production policy platform for DfT and Local Transport Authorities.

- 7-stage validated pipeline processing **1.75M GTFS trips** · 13,099 routes · 274,719 bus stops · 33,755 LSOAs (population 56.49M)
- Spatial join at **99.9993% match rate** · DuckDB warehouse serving 51 analytical sections through 27 Jinja2 templates
- Equity outcomes: **Gini 0.5741** · Palma ratio 5.702 · 4,245 zero-stop LSOAs · 5,189 evening-isolated communities (15.4%)
- ML: Random Forest Regressor · Isolation Forest · Gaussian Mixture Models · SHAP feature importance · 2SFCA accessibility scoring · DfT WebTAG v2.03fc BCR methodology
- FAISS RAG (sentence-transformers all-MiniLM-L6-v2) powering a React/Vite policy dashboard

`FastAPI` `DuckDB` `FAISS` `Python` `React` `GTFS` `Geospatial` `Public Policy`

---

### 📈 [Bharat Alpha](https://github.com/SVamseekar/bharat-alpha)
**Indian Equity Research Terminal · Jun 2024 – Present**

Hybrid RAG over 305 annual reports for 52 Nifty 50 companies — FAISS + BM25 + cross-encoder reranking (30 candidates → top 5), sector-aware routing, streaming Gemini 2.5 Flash responses with citation markers, live NSE prices via yfinance.

`FastAPI` `FAISS` `BM25` `Gemini` `React` `Supabase` `Python` `GCP`

---

### 🧾 [BillSathi](https://github.com/SVamseekar/billsathi)
**AI Bill Tracking Application · Aug 2024 – Present**

Multi-engine OCR pipeline (PaddleOCR + EasyOCR + OpenCV) → LightGBM classifier → ChromaDB semantic search → Gemini LLM fallback across 19 spending categories · 130 backend test cases · automated Google API email ingestion · Flutter frontend.

`Python` `FastAPI` `Flutter` `LightGBM` `ChromaDB` `Gemini` `OCR` `SQLite`

---

## 🛠️ Tech Stack

| Domain | Technologies |
|---|---|
| **AI & GenAI** | Google Vertex AI · Gemini · Google ADK · RAG · FAISS · BM25 · Cross-Encoder · LangChain · LLM Agents · PaddleOCR · scikit-learn · TensorFlow |
| **Cloud & Infra** | Azure Data Factory · Synapse Analytics · Databricks · Data Lake Gen2 · GCP Cloud Run · Docker · Kubernetes · GitHub Actions |
| **Data Engineering** | Python · PySpark · dbt · DuckDB · Apache Spark · ETL/ELT · Parquet · Pydantic · Power BI |
| **Backend** | Java 17 · Spring Boot 3 · FastAPI · Spring WebFlux · Spring Cloud Gateway · RabbitMQ · WebSockets · Flyway · OpenAPI |
| **Databases** | PostgreSQL · MongoDB · Redis · ChromaDB · Supabase · SQLite · DuckDB |
| **Frontend & Mobile** | TypeScript · React 18/19 · Next.js · React Native · Flutter · Redux Toolkit · shadcn/ui · Tailwind CSS |

---

## 🎓 Education & Certifications

| | |
|---|---|
| 🎓 **M.Sc. Data Science** — University of Greenwich, London · Merit | 2021 – 2022 |
| 🎓 **B.Tech. Electronics & Communication** — GITAM, Visakhapatnam · 8.3 CGPA | 2016 – 2020 |
| 📜 **Microsoft Azure Data Engineer Associate (DP-203)** | March 2025 |

---

## 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=SVamseekar&show_icons=true&theme=dark&hide_border=true&count_private=true" height="150"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=SVamseekar&layout=compact&theme=dark&hide_border=true" height="150"/>
</p>

---

<p align="center">
  <b>🇪🇺 EU Blue Card Eligible · Open to relocation · Germany · Netherlands · Ireland · Austria · wider EU</b><br/><br/>
  <a href="https://linkedin.com/in/souramarti">Connect on LinkedIn →</a>
</p>
