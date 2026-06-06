<h1 align="center">Marti Soura Vamseekar</h1>

<p align="center">
  <b>AI & Data Engineer · M.Sc. Data Science (University of Greenwich, UK, Merit) · Azure DP-203</b><br/>
  RAG/LLM pipelines · Event-driven microservices · Cloud data platforms<br/>
  📍 Hyderabad, India &nbsp;·&nbsp; 🇪🇺 <b>EU Blue Card Eligible</b> · Open to relocation across Germany, Netherlands, Ireland, Austria, and wider EU
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

AI and Data Engineer with production experience shipping RAG/LLM pipelines, event-driven microservices, and cloud data platforms. I work across Google Vertex AI, Java/Spring Boot, Python, dbt, DuckDB, Azure Data Factory, Databricks, and GCP — across fintech AI research, EU compliance analytics, and government-scale geospatial systems.

I build at real scale: a hybrid RAG system over 305 annual reports with FAISS + BM25 + cross-encoder reranking, a 6-service restaurant platform with a 12-country EU VAT engine and 399 API endpoints, a workforce intelligence platform confirming labour market tightness correlates with gender pay gaps (r ≈ +0.41) across 20 EU states, and a UK transport equity platform covering 56.5 million people across 33,755 LSOAs with a Gini coefficient of 0.5741.

Targeting EU-based **AI Engineer**, **Data Platform Engineer**, or **Software Engineer** roles where production system ownership, GenAI infrastructure depth, and EU regulatory awareness matter.

---

## 💼 Work Experience

### Freelance Software Developer — [Innosolv Private Limited](https://innosolv.com)
**London, UK (Remote) · Oct 2025 – May 2026**

*UK-based fintech delivering algorithmic trading and AI-powered equity research for NSE cash and F&O markets.*

- Designed and delivered a **unified algorithmic trading platform** (Java 17, Spring Boot 3.2, MongoDB, WebFlux) integrating Zerodha Kite Connect for live NSE equity and derivatives market data, order execution, and position management
- Built an **options analytics engine** covering Iron Condor strategy, spread margin calculation, basket orders, and open interest analysis — enabling automated multi-leg derivatives execution
- Engineered an **async order pipeline** with Bucket4j rate limiting to meet Zerodha API constraints, sustaining reliable high-frequency order submission without throttling
- Delivered a **high-frequency trading module** with real-time moving average signals, participant-wise OI tracking, and MongoDB-persisted trade history

`Java 17` `Spring Boot 3.2` `MongoDB` `WebFlux` `Zerodha Kite Connect` `Bucket4j` `HFT`

---

## 🚀 Key Projects

### 📊 [WorkforceGuard AI](https://github.com/SVamseekar/workforceguardai)
**EU Pay Transparency & Workforce Intelligence Platform · Jan 2024 – Present**

European workforce intelligence and compliance platform for HR and compensation teams, built for the EU Pay Transparency Directive 2023/970 (transposition deadline June 2026).

- **Confirmed r ≈ +0.41 correlation** between labour market tightness and gender pay gaps across 20 EU member states — grounding pay-transparency compliance analysis in statistical evidence
- **26-model dbt pipeline** (staging → marts) over 16 Eurostat datasets (LFS, JVS, SES, NACE), ESCO occupation taxonomy (v1.2.1), and France public company data — ingesting EU27 labour market signals across 27 countries
- **7 ML models** trained on 32,769 samples for employee access prediction; Random Forest achieved **94.7% accuracy, AUC 0.855** on a 912K-record test set
- **4 composite workforce indices** — Hiring Pressure Index, Labour Resilience, Equity Risk Score, Transition Readiness — all formula-versioned, human-review-flagged, and audit-traceable
- FastAPI analytics backend + React 19 dashboard with evidence packs, governance event log, and pay-transparency category-review simulation (classifying worker categories as `justified_difference`, `observed_gap`, or `unresolved_review_item`)

`dbt` `DuckDB` `FastAPI` `React 19` `scikit-learn` `Eurostat API` `ESCO` `GitHub Actions` `EU Compliance`

---

### 🍽️ [Masova Platform](https://github.com/SVamseekar/masova-platform)
**Cloud-Native Restaurant Management System · Feb 2023 – Present**

Full-stack, multi-channel restaurant management platform: customer ordering (web + mobile), kitchen operations, delivery, staff management, analytics, and AI-powered decision support.

- **6 Spring Boot 3 / Java 21 microservices** on GCP Cloud Run exposing **399 API endpoints** across order management, payments, logistics, and BI — with Spring Cloud Gateway handling JWT auth, per-route rate limits, and reactive routing
- **12-country EU VAT engine** with context-aware rates (Germany TSE, France NF525, Italy SDI, Spain VeriFactu, UK HMRC MTD, US state tax) and fiscal signing triggered on order completion
- **Event-driven order pipeline** via RabbitMQ, propagating real-time state to all clients over WebSockets (STOMP/SockJS) with <100ms state-change delivery · dual-write MongoDB + PostgreSQL with Flyway migrations
- **8 Google ADK 1.25 / Gemini agents** (demand forecasting, churn prevention, inventory reorder, review response) with 9 callable tools, Redis session management (DB 1, 1h TTL), and LLM fallback to rule-based logic
- **3 production frontends** — React 19 web, React Native 0.83 staff app (MaSoVa Crew), React Native 0.81 customer app — with Stripe/Razorpay, real-time GPS tracking, and offline-first Redux Persist
- GDPR-compliant customer data layer: RLS, data retention policies (2-year customer, 7-year PCI), SAR/DPR/portability workflows

`Spring Boot 3` `Java 21` `GCP Cloud Run` `Spring Cloud Gateway` `RabbitMQ` `MongoDB` `PostgreSQL` `Redis` `Google ADK` `Gemini` `React Native` `GDPR`

---

### 🚌 [Aequitas](https://github.com/SVamseekar/aequitas)
**UK Bus Transport Policy Intelligence Platform · Oct 2021 – Mar 2022 · Extended Mar 2026 – Present**

M.Sc. dissertation (University of Greenwich) extended into a production policy analytics platform for the Department for Transport and Local Transport Authorities.

- **7-stage validated pipeline** processing 274,719 active NaPTAN bus stops, 13,099 BODS GTFS routes, 1.75M trips across 33,755 English LSOAs (56.49M population) — 19 quality notebooks, 103 checks, 0 failures
- **Equity findings**: Gini coefficient **0.5741** (exceeds UK income inequality at 0.36) · Palma ratio 5.702 · Concentration Index +0.1358 (pro-rich) · 4,245 zero-stop LSOAs · 5,189 evening-isolated communities (15.4%) · 612 triple-deprived LSOAs
- **ML layer**: Random Forest Regressor (R² 0.472) · HDBSCAN + GMM clustering · Isolation Forest anomaly detection · SHAP feature importance (top predictor: `nocar_pct`) · 2SFCA accessibility scoring
- **51 analytical sections** across 8 policy dimensions, served via DuckDB warehouse + 30 Jinja2 narrative templates across 30 regional/urban-rural filter combinations
- **Production platform**: FastAPI backend + FAISS RAG chatbot (sentence-transformers all-MiniLM-L6-v2 + Gemini 2.5 Flash) + React/TypeScript/shadcn-ui frontend · DfT WebTAG v2.03fc BCR methodology for economic appraisal

`FastAPI` `DuckDB` `FAISS` `Gemini 2.5 Flash` `Python 3.12` `GeoPandas` `GTFS` `SHAP` `React` `TypeScript` `Public Policy`

---

### 📈 [Bharat Alpha](https://github.com/SVamseekar/bharat-alpha)
**Indian Equity Research Terminal · Jun 2024 – Present**

AI-powered research terminal combining hybrid RAG over 305 annual reports with fundamental equity analysis across 52 Nifty 50 companies (FY2020–FY2025).

- **Hybrid RAG pipeline**: FAISS IndexFlatIP + BM25Okapi lexical retrieval + sector-aware routing → cross-encoder reranking (30 candidates → top 5) over **143K chunks** embedded with `gemini-embedding-001`
- **Streaming Gemini 2.5 Flash** responses with numbered citation markers (`[N]`) traceable to source filings · structured report format (Business Overview → Financial Health → Verdict) for fact-sheet queries
- Full-stack: React 18 + TypeScript + shadcn/ui · Supabase auth + Postgres conversation history · live NSE prices via yfinance (5-min cache) · investment journal with AI critique and thesis re-evaluation

`FastAPI` `FAISS` `BM25` `Gemini 2.5 Flash` `gemini-embedding-001` `React 18` `TypeScript` `Supabase` `Python 3.11`

---

### 🧾 [BillSathi](https://github.com/SVamseekar/billsathi)
**AI Bill Tracking Application · Aug 2024 – Present**

Local-first, privacy-first bill tracking app for Indian households with OCR capture, ML categorisation, and LLM-powered insights.

- **Multi-engine OCR pipeline**: PaddleOCR 2.9.1 primary + EasyOCR fallback (confidence gate 0.60) + OpenCV preprocessing (5-stage: denoise → adaptive threshold → deskew → sharpen) with vendor-specific parsers for Swiggy, Zomato, Amazon, Blinkit, Zepto, Rapido
- **Hybrid categorisation engine** (19 spending categories): rule-based → SGDClassifier (HashingVectorizer, partial_fit) → ChromaDB semantic search → Gemini 2.0 Flash Lite fallback; activated by correction count thresholds (20+ → ML, 50+ → semantic)
- **48 API endpoints** across bill ingestion, correction, price history, alerts, email parsing, Razorpay transaction matching, and Google Drive backup; circuit breaker on Gemini (3 consecutive 429s → 5-min cooldown)
- Flutter frontend (flutter_riverpod, go_router, fl_chart) · Cloudflare Zero Trust Tunnel · Oracle Cloud Free Tier deployment

`Python` `FastAPI` `Flutter` `PaddleOCR` `LightGBM` `ChromaDB` `Gemini` `SQLite` `Docker` `Cloudflare`

---

## 🛠️ Tech Stack

| Domain | Technologies |
|---|---|
| **AI & GenAI** | Google Vertex AI · Gemini 2.5 Flash · Google ADK 1.25 · RAG · FAISS · BM25 · Cross-Encoder · SHAP · PaddleOCR · scikit-learn · TensorFlow · LangChain |
| **Cloud & Infra** | GCP Cloud Run · Firebase Hosting · Azure Data Factory · Synapse Analytics · Databricks · Data Lake Gen2 · Docker · GitHub Actions |
| **Data Engineering** | Python 3.12 · PySpark · dbt · DuckDB · Apache Spark · Parquet · Pandas · GeoPandas · ETL/ELT · Power BI |
| **Backend** | Java 21 · Spring Boot 3 · FastAPI · Spring WebFlux · Spring Cloud Gateway · RabbitMQ · WebSockets · Flyway · OpenAPI |
| **Databases** | PostgreSQL · MongoDB · Redis · ChromaDB · Supabase · SQLite · DuckDB |
| **Frontend & Mobile** | TypeScript · React 18/19 · React Native 0.83 · Flutter · Redux Toolkit · shadcn/ui · Tailwind CSS · Recharts |

---

## 🎓 Education & Certifications

| | |
|---|---|
| 🎓 **M.Sc. Data Science** — University of Greenwich, London · **Merit** · Dissertation: UK Bus Data Analysis | 2021 – 2022 |
| 🎓 **B.Tech. Electronics & Communication** — GITAM Institute, Visakhapatnam · **8.3 CGPA** · Dissertation: Hyperspectral Image Analysis | 2016 – 2020 |
| 📜 **Microsoft Certified: Azure Data Engineer Associate (DP-203)** · Credential: 2CEA6999835BAD6E | March 2025 |

---

## 📊 GitHub Activity

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=SVamseekar&show_icons=true&theme=dark&hide_border=true&include_all_commits=true" height="150"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=SVamseekar&layout=compact&theme=dark&hide_border=true&langs_count=8" height="150"/>
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=SVamseekar&theme=dark&hide_border=true" height="150"/>
</p>

---

<p align="center">
  <b>🇪🇺 EU Blue Card Eligible · Open to relocation · Germany · Netherlands · Ireland · Austria · wider EU</b><br/><br/>
  <a href="https://linkedin.com/in/souramarti">Connect on LinkedIn →</a> &nbsp;·&nbsp; <a href="mailto:martisoura@gmail.com">martisoura@gmail.com</a>
</p>
