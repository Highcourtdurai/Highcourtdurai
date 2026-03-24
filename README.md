# Hi, I'm Charunya 👋

I build end-to-end AI and ML systems — from classical machine learning and deep learning to RAG pipelines, agentic AI, MCP servers, and production-deployed applications. My projects span Computer Vision, NLP, Generative AI, Time Series, and MLOps.

---

## 🚀 Featured Projects

### 🤖 Agentic AI & GenAI Applications

- [AI DevOps Co-pilot](https://github.com/Charu305/devops-copilot) — Production MCP server that connects Claude AI to GitHub, Jira, and Slack via 17 custom tools with a Gemini 2.0 Flash reasoning layer. Automates standup generation, sprint health scoring, PR risk analysis, and incident response from a single conversational interface.

- [AI Resume Screening App](https://github.com/Charu305/ai-resume-screening) — Multi-agent Gemini LLM application that screens resumes against a job description using a JD Analyser → Resume Evaluator → Ranking Agent pipeline. Built with modular agents, centralised prompt templates, and Dockerised for deployment.

- [Meeting Intelligence](https://github.com/Charu305/meeting-intelligence) — Supervisor agent system that transforms meeting transcripts into structured intelligence reports — summary, action items, decisions, and sentiment — with automated email delivery via SMTP. Dockerised with a 4-agent architecture.

- [RAG with AI Agents](https://github.com/Charu305/Simple-RAGwithAgents) — AutoGen multi-agent RAG system over an Employee Handbook PDF. Agents autonomously plan retrieval steps, handle multi-hop questions, and coordinate through a turn-based conversation loop. Configured via OAI_CONFIG_LIST.json.

- [Multi-Doc Assistant](https://github.com/Charu305/Multi-Doc-Assistant) — Multi-document RAG application with persistent user memory across sessions (user_memory.json). FastAPI backend with cross-document retrieval, per-chunk source attribution, and memory-augmented prompt construction. Dockerised.

- [Simple RAG](https://github.com/Charu305/Simple-RAG) — End-to-end RAG pipeline over a Company HR Policy Handbook PDF. Covers document loading, chunking with overlap, embedding generation, FAISS vector store, and grounded LLM answer generation with hallucination prevention.

- [Text-to-SQL App](https://github.com/Charu305/Text-to-SQL-APP) — LLM application that translates natural language questions into executable SQL queries against a SQLite database. Schema-aware prompting, generated SQL displayed alongside results for transparency. Dockerised with database seeded at build time.

- [Hotel Chatbot](https://github.com/Charu305/Hotel-Chatbot) — NLP-powered hotel assistant with intent classification across 8 guest query categories, dynamic FoodMenu.json retrieval, and a modular utils.py utility layer. Handles fallback for unrecognised inputs.

---

### 👁️ Computer Vision & Deep Learning

- [Real-Time Face Mask Detection](https://github.com/Charu305/Face-Mask) — Two-stage deep learning pipeline combining RetinaFace (PyTorch) for face detection and MobileNetV2 (Keras) for mask classification. Evaluated on WiderFace (94.82% easy) and FDDB (99.22%) benchmarks. Includes real-time webcam inference and ONNX export.

- [Helmet Detection — YOLOv5 / YOLOv8](https://github.com/Charu305/Helmet-Detection) — Real-time safety helmet detection using fine-tuned YOLOv5s and YOLOv8s on a custom YOLO-format annotated dataset. Includes dataset splitting, data.yaml configuration, training output diagnostics, and live webcam inference.

---

### 📝 NLP & Text Classification

- [Fake News Detection — LSTM](https://github.com/Charu305/Fake-News-Prediction) — Binary text classifier that identifies fake vs. real news articles using an LSTM with a learned Embedding layer. Full NLP preprocessing pipeline: lowercasing, stopword removal, stemming, Keras tokenisation, and sequence padding.

---

### 📈 Time Series & Financial Analytics

- [Domino's Pizza Sales Forecasting](https://github.com/Charu305/Dominos-Pizza-Sales) — SARIMA model with auto parameter tuning (AIC-based) on historical pizza sales data. Translates the sales forecast into an ingredient procurement plan via a pizza-ingredient lookup table — outputting predicted_ingredient_totals.csv.

- [Stock Price Analysis & Prediction](https://github.com/Charu305/Stocks-Price) — Financial time series analysis with engineered technical indicators (SMA, EMA, RSI, MACD, Bollinger Bands) and LSTM-based price forecasting. Covers return distributions, volatility clustering, and backtesting discipline.

- [Netflix Subscriber Growth Analysis](https://github.com/Charu305/Netflix-Subscribers) — Quarterly subscriber trend analysis with regional breakdown (UCAN, EMEA, LATAM, APAC), QoQ and YoY growth rates, S-curve growth modelling, and subscriber count forecasting.

---

### 🤖 Classical Machine Learning

- [Used Car Price Prediction — HopeAI](https://github.com/Charu305/HopeAI-Car_price_prediction) — End-to-end regression pipeline with feature engineering (car_age), model comparison (Linear Regression, Decision Tree, Random Forest, XGBoost), and Streamlit deployment. Best R² ~0.92 with Random Forest.

- [Loan Approval Prediction — HopeAI](https://github.com/Charu305/Loan-Approval-Prediction) — Binary classification pipeline for loan approval decisions. Log transformation on skewed income features, credit history as dominant predictor, evaluated with F1 Score and ROC-AUC. Best F1 ~0.84 with Random Forest.

---

## 🔧 What I worked on — Agentic AI & GenAI

- [MCP Server — 17 tools across GitHub, Jira, Slack](https://github.com/Charu305/devops-copilot/tree/master/tools) — Lazy loading, Jira workflow transitions with fuzzy matching, stdout protection for JSON-RPC
- [Supervisor Agent — Meeting Intelligence](https://github.com/Charu305/meeting-intelligence/blob/master/Supervisor.py) — Orchestrates Summariser, Action Extractor, Decision Extractor, Sentiment Analyser agents
- [AutoGen Multi-Agent RAG](https://github.com/Charu305/Simple-RAGwithAgents/blob/main/AI_Agents.ipynb) — RAG as a callable tool, UserProxyAgent + AssistantAgent coordination, multi-hop retrieval
- [Multi-Agent Resume Screening](https://github.com/Charu305/ai-resume-screening/tree/master/agents) — JD Analyser → Resume Evaluator → Ranking Agent with centralised prompt templates
- [Persistent User Memory](https://github.com/Charu305/Multi-Doc-Assistant/blob/master/user_memory.json) — Session-persistent user context injected into RAG prompts across sessions
- [Schema-aware Text-to-SQL](https://github.com/Charu305/Text-to-SQL-APP/blob/master/app.py) — Database schema injected into every LLM prompt for reliable SQL generation

---

## 🔧 What I worked on — Computer Vision

- [RetinaFace face detector training](https://github.com/Charu305/Face-Mask/blob/main/train.py) — WiderFace benchmark, MobileNet0.25 and ResNet-50 backbones, FDDB evaluation
- [MobileNetV2 mask classifier](https://github.com/Charu305/Face-Mask/blob/main/train_mobilenetv2_mask.py) — Transfer learning on cropped face dataset, saved as .h5
- [ONNX export for edge deployment](https://github.com/Charu305/Face-Mask/blob/main/convert_to_onnx.py) — Cross-platform model export for C++, mobile, and hardware accelerators
- [YOLOv5 / YOLOv8 custom training](https://github.com/Charu305/Helmet-Detection/blob/main/Train_images.py) — Custom YOLO-format dataset, data.yaml config, runs/detect/train diagnostics
- [Real-time webcam detection](https://github.com/Charu305/Helmet-Detection/blob/main/Train_wecam.py) — Live bounding box overlays on helmet/no-helmet detections

---

## 🔧 What I worked on — NLP & Time Series

- [LSTM fake news classifier](https://github.com/Charu305/Fake-News-Prediction/blob/main/Fake%20News%20-%20LSTM.ipynb) — Embedding layer + LSTM + Dropout, text preprocessing pipeline, F1 Score evaluation
- [SARIMA sales forecasting](https://github.com/Charu305/Dominos-Pizza-Sales/blob/main/Pizza_Sales.ipynb) — ADF stationarity test, AIC-based parameter tuning, ingredient procurement output
- [Intent classification chatbot](https://github.com/Charu305/Hotel-Chatbot/blob/main/Hotel-Chatbot.ipynb) — 8 intents, training utterance variety, fallback threshold, FoodMenu.json integration

---

## 🛠️ Skills & Tools

- **Languages:** Python
- **Agentic AI / GenAI:** MCP Protocol, AutoGen, LangChain, RAG, Prompt Engineering, Gemini 2.0 Flash, OpenAI GPT
- **Deep Learning:** PyTorch, TensorFlow, Keras, LSTM, MobileNetV2, RetinaFace, YOLOv5, YOLOv8
- **ML / Data:** Scikit-learn, XGBoost, SARIMA, Pandas, NumPy
- **Computer Vision:** OpenCV, ONNX, WiderFace Evaluation, FDDB
- **NLP:** NLTK, Sentence Transformers, FAISS, ChromaDB, TF-IDF
- **APIs & Integrations:** GitHub API (PyGithub), Jira Cloud API, Slack API, Gmail SMTP, SQLite
- **Deployment:** Docker, FastAPI, Uvicorn, Streamlit, Flask
- **Environment:** Jupyter Notebook, Git, Anaconda

---

## 📬 Connect with Me

- [GitHub — Charu305](https://github.com/Durai)
