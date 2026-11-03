<h1 align="center">Prajakth N Kumar</h1>

<p align="center">
  <b>Full-stack and AI engineer</b><br/>
  Computer Science student at B.M.S.C.E, Bangalore<br/>
  <i>Veni. Vidi. Vici.</i>
</p>

<p align="center">
   <a href="https://vercel.app"><b>Portfolio</b></a> &nbsp;&nbsp;•&nbsp;&nbsp;
   <a href="https://linkedin.com"><b>LinkedIn</b></a> &nbsp;&nbsp;•&nbsp;&nbsp;
   <a href="mailto:prajakth.kumar@gmail.com"><b>Email</b></a>
</p>


---

## About

I build AI systems end to end: the model, the retrieval or inference pipeline around it, and the interface that puts it in front of users. My work spans three areas: LLM and agent tooling, applied machine learning on physical and acoustic signals, and full-stack products with real deployments.

I prefer designs where deterministic logic owns the critical decisions and the model handles interpretation. This pattern runs through Meridian, FraudLens, IntelliRepo and the notification router below.

---

## Highlights

| | |
| :-- | :-- |
| **Published research** | LSTM-PINN framework for battery state-of-health prediction, published in *Scientific Reports* (2026). |
| **Fraud detection** | FraudLens reaches 0.9477 AUC-ROC on a locked held-out set of 88,581 transactions, trained on 590,540 IEEE-CIS records. |
| **Hardware to inference** | PRISM spans ESP32 firmware, audio capture, ML detection and a mobile companion app. |
| **Live deployments** | [FraudLens](https://fraudlens-lyart.vercel.app/), [Skill Exchange 2.0](https://skill-exchange-htcsaefxdfe8g2fv.southeastasia-01.azurewebsites.net) and my [portfolio](https://prajakth-portfolio.vercel.app/). |
| **Hackathons** | iQOO Hackathon 2026 finale (Rookie), Razorpay AI buildathon (FraudLens), HackerRank Orchestrate (notification router). |

---

## Research

**[A temperature- and impedance-aware LSTM-PINN framework for physically consistent battery SOH prediction](https://doi.org/10.1038/s41598-026-37850-y)**
*Scientific Reports*, vol. 16, 2026. Co-authored with P. R. Upadhya, S. Nischay and others.

A physics-informed neural network combined with an LSTM to predict battery state of health on the NASA battery cycling dataset. The model enforces Arrhenius temperature dependence and impedance-based degradation (electrolyte and charge transfer resistance) through custom physics loss terms, with Bayesian hyperparameter search using Optuna. Code: [PINN-based-Hybrid-LSTM-Architecture-for-Battery-Degradation](https://github.com/praju120056/PINN-based-Hybrid-LSTM-Architecture-for-Battery-Degradation).

**[Facial Emotion Recognition Framework](https://github.com/praju120056/Facial-Emotion-Recognition-Framework)** (in development)
An extension of Antoine Lame's GazeTracking that combines gaze direction and facial features with a PyTorch CNN, aimed at learner states such as frustration and confusion on top of the base emotions.

---

## Selected projects

### AI systems and agents

| Project | Description | Stack |
| :-- | :-- | :-- |
| [**FraudLens**](https://github.com/praju120056/FraudLens) | Payment risk intelligence console for merchants. Scores Razorpay payloads with an XGBoost model, explains each decision with TreeSHAP, synthesizes evidence with Gemini and writes an immutable audit trail. The ML model stays the sole decision-maker. [Live demo](https://fraudlens-lyart.vercel.app/). | ![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white) ![XGBoost](https://img.shields.io/badge/-XGBoost-189AB4?style=flat-square) ![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) |
| [**IntelliRepo**](https://github.com/praju120056/IntelliRepo) | Repository intelligence engine. Builds dependency and call graphs from Python ASTs, indexes code with embeddings, and answers structural questions (callers, dependencies, impact of a change) with graph-aware retrieval before any LLM is involved. | ![FastAPI](https://img.shields.io/badge/-FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![ChromaDB](https://img.shields.io/badge/-ChromaDB-262626?style=flat-square) ![React](https://img.shields.io/badge/-React-61DAFB?style=flat-square&logo=react&logoColor=black) ![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) |
| [**Meridian**](https://github.com/praju120056/Meridian) | Agent that watches GitHub pull requests, decides which ones deserve attention and routes alerts through Caspian to Slack and Telegram. HMAC-verified webhooks, deterministic severity policy, Gemini 2.5 Flash for semantic assessment, and a rule that the LLM can never downgrade a deterministic HIGH. Tested against [meridian-demo](https://github.com/praju120056/meridian-demo). | ![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white) ![FastAPI](https://img.shields.io/badge/-FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white) |
| [**Rookie**](https://github.com/praju120056/rookie) | iQOO Hackathon 2026 finale entry (Team OGs). AI personas test an app the way real users would, such as a 65-year-old new to smartphones or a user on a slow 2G network. The personas change what the model can actually perceive, and a Streamlit report shows where each one got stuck. Runs fully locally with Gemma 3 through Ollama. | ![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Playwright](https://img.shields.io/badge/-Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white) ![Streamlit](https://img.shields.io/badge/-Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white) |
| [**Notification Router**](https://github.com/praju120056/hackerrank_aug27) | HackerRank Orchestrate entry. Routes WhatsApp messages (text, images, voice notes) to notify, digest or mute using a deterministic-first pipeline: rule engine, tiered evidence retrieval, then batched Gemini decisions with checkpointing and a 50-test offline suite. | ![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Gemini](https://img.shields.io/badge/-Gemini-8E75B2?style=flat-square) |
| [**llm-powered-rag**](https://github.com/praju120056/llm-powered-rag) | RAG system with PDF and recursive website ingestion, pgvector similarity search, Groq-hosted Llama 3.3 for generation, and a separate admin dashboard for ingestion. | ![Flask](https://img.shields.io/badge/-Flask-000000?style=flat-square&logo=flask&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![LangChain](https://img.shields.io/badge/-LangChain-1C3C3C?style=flat-square) |

### Embedded systems and applied ML

| Project | Description | Stack |
| :-- | :-- | :-- |
| [**PRISM Smart Inhaler**](https://github.com/praju120056/PRISM-Smart-Inhaler) | Acoustic monitoring for pressurised metered-dose inhalers. Classifies 200 ms audio windows into drug, inhale, exhale and noise events, then assesses each inhalation against a one-sided 95% reference limit. Evaluated with grouped cross-validation across Random Forest, SVM, XGBoost and a 1D CNN exported to ONNX. Research stage, not a clinical classifier. | ![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white) ![scikit-learn](https://img.shields.io/badge/-scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white) ![PyTorch](https://img.shields.io/badge/-PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white) ![ONNX](https://img.shields.io/badge/-ONNX-005CED?style=flat-square&logo=onnx&logoColor=white) |
| [**PRISM Hardware**](https://github.com/praju120056/prism-hardware) | Capture layer for PRISM. ESP32 firmware reads an INMP441 I2S MEMS microphone at 8 kHz and streams raw samples over serial. Host scripts verify CRC-32, bit alignment and sample rate, then produce WAV files. | ![C++](https://img.shields.io/badge/-C++-00599C?style=flat-square&logo=cplusplus&logoColor=white) ![ESP32](https://img.shields.io/badge/-ESP32-E7352C?style=flat-square&logo=espressif&logoColor=white) |
| [**NeoCocoon**](https://github.com/praju120056/neococoon) | Smart baby incubator prototype. A Raspberry Pi touchscreen UI talks over serial to a Pico that reads temperature, humidity and light sensors and drives heaters, humidifiers and phototherapy lamps. | ![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Raspberry Pi](https://img.shields.io/badge/-Raspberry_Pi-A22846?style=flat-square&logo=raspberrypi&logoColor=white) |
| [**Robotics**](https://github.com/praju120056/Robotics) | Obstacle-avoidance robot in a PyBullet simulation that steers using simple front, left and right sensing. | ![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white) |

### Full-stack and security

| Project | Description | Stack |
| :-- | :-- | :-- |
| [**Skill Exchange 2.0**](https://github.com/praju120056/skill-exchange-2.0) | Student skill-sharing platform with aggregation-based skill matching, Socket.IO direct messaging, a Gemini-powered AI mentor, JWT auth in HttpOnly cookies and Google OAuth. Deployed on Azure with a GitHub Actions pipeline. [Live](https://skill-exchange-htcsaefxdfe8g2fv.southeastasia-01.azurewebsites.net). | ![React](https://img.shields.io/badge/-React-61DAFB?style=flat-square&logo=react&logoColor=black) ![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![Node.js](https://img.shields.io/badge/-Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white) ![MongoDB](https://img.shields.io/badge/-MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white) |
| [**Banking ZTA**](https://github.com/praju120056/banking_zta) | Zero Trust banking simulation: mTLS device verification at Nginx, Keycloak for identity and roles, Open Policy Agent for per-transaction risk scoring, and TOTP step-up for high-risk transfers. Forked from a teammate's repository. | ![FastAPI](https://img.shields.io/badge/-FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white) |
| [**AQI Detector**](https://github.com/praju120056/AQI) | Air quality dashboard backed by the OpenWeatherMap API with MongoDB Atlas storage. | ![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white) ![MongoDB](https://img.shields.io/badge/-MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white) |
| [**Blog Web App**](https://github.com/praju120056/blog_web) | Server-rendered blog with full CRUD, EJS templates and a React like button. | ![Express](https://img.shields.io/badge/-Express-000000?style=flat-square&logo=express&logoColor=white) ![MongoDB](https://img.shields.io/badge/-MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white) |
| [**Portfolio**](https://github.com/praju120056/portfolio) | Minimal single-page portfolio with a terminal-style component, built to prioritise content over decoration. [Live](https://prajakth-portfolio.vercel.app/). | ![React](https://img.shields.io/badge/-React-61DAFB?style=flat-square&logo=react&logoColor=black) ![Vite](https://img.shields.io/badge/-Vite-646CFF?style=flat-square&logo=vite&logoColor=white) |

### Systems and coursework

| Project | Description |
| :-- | :-- |
| [**UNIX-style-shell**](https://github.com/praju120056/UNIX-style-shell) | Shell in C using `fork` and `execvp`, with built-in `cd`, `exit` and `clear`. |
| [**java-tetris**](https://github.com/praju120056/java-tetris) | JavaFX Tetris clone adapted from an open-source project. |
| [**devops**](https://github.com/praju120056/devops) | Ten exercises from the seventh-semester DevOps course, each with its own README. |
| [**soa_lab**](https://github.com/praju120056/soa_lab) | Service-oriented architecture lab exercises. |

---

## Currently

- Developing **Meridian**, **PRISM** and **IntelliRepo**
- Preparing the **Facial Emotion Recognition Framework** for publication
- Taking the **Banking ZTA** system toward deployment

## Interests

Backend engineering, distributed systems, AI and ML systems, operating systems, embedded systems.

---

### Languages

<p>
  <img src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white"/>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black"/>
  <img src="https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white"/>
</p>

### Backend & APIs

<p>
  <img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white"/>
  <img src="https://img.shields.io/badge/Express.js-000000?style=flat-square&logo=express&logoColor=white"/>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"/>
  <img src="https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white"/>
  <img src="https://img.shields.io/badge/REST_APIs-02569B?style=flat-square"/>
</p>

### AI & Machine Learning

<p>
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white"/>
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white"/>
  <img src="https://img.shields.io/badge/XGBoost-189AB4?style=flat-square"/>
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white"/>
  <img src="https://img.shields.io/badge/LLMs-412991?style=flat-square"/>
</p>

### Databases & Infrastructure

<p>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white"/>
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black"/>
  <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white"/>
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white"/>
</p>


---

## GitHub at a glance


<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://streak-stats.demolab.com?user=praju120056&hide_border=true&theme=github-dark-blue"/>
    <img alt="Contribution streak" src="https://streak-stats.demolab.com?user=praju120056&hide_border=true"/>
  </picture>
</p>


---

<p align="center">
  <sub>Open to internships and collaborations. Reach me through <a href="https://www.linkedin.com/in/prajakth-n-kumar-0092902a6">LinkedIn</a> or my <a href="https://prajakth-portfolio.vercel.app/">portfolio</a>.</sub>
</p>
