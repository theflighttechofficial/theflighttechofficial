# S. Varun Vaibhav

**AI & Data Analytics engineer. I build data pipelines, ML systems, and full-stack products.**

3rd-year B.Tech CSE (AI & Data Analytics), Sri Ramachandra Institute of Higher Education and Research (SRIHER), Chennai. CGPA 7.8/10. Expected 2028.
Targeting an MS in Computer Science / Data Science at Arizona State University (Fall 2029).

---

## About

I turn manual, repetitive work into systems that run on their own. My biggest production result so far is a document-extraction pipeline built at L&T Construction. It cut a 3–4 day manual process to about 15 minutes per run and dropped LLM cost per run from about $22 to $2.

I work across three layers:
- **Data and ML:** Python, pandas, scikit-learn, XGBoost, SHAP, YOLOv8, OpenCV, RAG pipelines
- **Product engineering:** TypeScript, React, Vite, Tailwind, Node.js, Express, FastAPI
- **Data stores:** SQL, PostgreSQL, MongoDB, Supabase, FAISS

I prefer shipping working systems with real users over prototypes that only run in notebooks.

---

## Experience

**Data Analyst Intern, Larsen & Toubro (L&T) Construction, Data Analytics Department**
*May 2026 – Jul 2026 · Chennai*
- Built a hybrid RAG pipeline (FAISS + BM25, merged with Reciprocal Rank Fusion) that extracts structured data from 1,200+ page tender PDFs into Excel workbooks.
- Used GPT-4o for extraction and GPT-4o-mini for verification. Added parallel processing with ThreadPoolExecutor.
- Cut cost per run from about $22 to $2 with offline SentenceTransformer embeddings, caching, and rule-based check skipping.
- Built **Scan2Sheet**, a Tesseract OCR tool that extracts feeder and panel schedules from AutoCAD single-line diagram PDFs with no embedded text.
- Received a letter of recommendation from the department.
- Source code is confidential to L&T. The public repositories show documentation only.

**Web Design & Development Intern, Neoshaan Technologies (OPC) Pvt. Ltd.**
*May 2025 – Jul 2025 · Remote*
- Rebuilt the company website in React, Vite, and Tailwind CSS: home, services, course catalog, course detail pages, careers, and contact.
- Built a contact and job-application form backend with Node.js and Nodemailer.
- Fixed mobile layout problems across three client sites and logged UX defects during an audit.

---

## Featured Projects

### Production and client work

**[Paws & Care Clinic](https://deivayanaipetclinic.online)** · [repo](https://github.com/theflighttechofficial/Paws-Care-a-unit-of-deivayanai-pet-clinic)
Full-stack platform for a veterinary clinic, live in production. Pet owners book appointments with payment-gated slots. Doctors and admins manage pet health records and schedules. Integrations: Razorpay payments, Google Calendar and Meet, and transactional email through Resend.
*Stack:* React, Tailwind CSS, Node.js, Express, PostgreSQL, Google APIs, Razorpay, Resend

**[Anchora](https://github.com/theflighttechofficial)** · *private repository*
SaaS that combines a freelancer project workspace with a startup ecosystem. About 60 routes, 30 database migrations, and 5 user roles. AI features run through Supabase Edge Functions: co-founder matching, investor matching, pitch analysis, proposal generation, and contract summaries.
*Stack:* React, TypeScript, Zustand, Supabase, PostgreSQL, GPT-4o-mini

### Applied AI and computer vision

**[Road-AI](https://github.com/theflighttechofficial/RoadAi-Building-better-roads-for-India)**
Full pipeline for road damage detection, from raw images, video, or drone footage to repair tickets with QR codes.
- Ensemble of YOLOv8 models, including a fine-tuned road-damage model.
- Temporal fusion across video frames to reduce false positives. Monte Carlo Dropout to flag low-confidence detections.
- Depth estimation from shadow gradients, without LiDAR.
- Repair cost estimates based on Tamil Nadu PWD and NHAI schedules of rates.
- Mean average precision mAP50 of 0.648 on RDD2022, with 38% fewer false positives.
- Presented at SRIHER Research Day 2026. Submitted to an IIT Madras hackathon.
*Stack:* Python, YOLOv8, OpenCV

**[DocuMind AI](https://github.com/theflighttechofficial/DocuMind-Hybrid-RAG-based-Doc-analyzer)** · *in development*
Evidence-first document Q&A for PDF, DOCX, and TXT files. Every answer cites the page and passage it came from. If the document does not contain the answer, the system says so instead of guessing. Includes classic NLP analysis (NER, POS tagging, keyword extraction, readability) alongside the RAG pipeline.
*Stack:* FastAPI, React, Vite, sentence-transformers, FAISS

**[Ghost Patterns v2](https://github.com/theflighttechofficial/Ghost-Patterns)** · data mining project
Tests whether a mined pattern is real or just noise. Runs the same mining pipeline on null models, such as shuffled data, Gaussian-matched data, and Curveball swap randomization, then calibrates real findings against those baselines. Also detects leakage (functional dependencies, row-order artifacts, duplicate encodings) before mining.
*Stack:* Python

**[AI-Powered Financial Affordability Agent ("Buy or Wait")](https://github.com/theflighttechofficial/AI-Powered-Financial-Affordability-Agent)**
Estimates whether a user can afford a purchase by forecasting a 90-day cash-flow timeline. The arithmetic runs in deterministic code; LLMs handle only extraction. Groq is the primary model. A local Ollama model is the fallback. Receipt images go to a local vision model. The agent treats messages and images as untrusted input.
*Stack:* Python, Groq API, Ollama

**[MessageMind: WhatsApp Notification Router](https://github.com/theflighttechofficial/MessageMind)** · HackerRank Orchestrate, Aug 2026
Routes incoming WhatsApp messages (text, poster images, voice notes) into one of three actions: notify now, digest later, or mute as spam or unsafe. Result: 75% action accuracy and 83% type accuracy on 110 messages.
*Stack:* Python, Groq API (llama-3.1-8b-instant)

**[AgriYield AI](https://github.com/theflighttechofficial/AgriYield-Ai-Pro)** · published on Kaggle
Crop yield prediction from soil nutrients and weather. XGBoost with SHAP explanations for each prediction, what-if analysis for fertilizer changes, and downloadable PDF reports.
*Stack:* Python, XGBoost, SHAP, scikit-learn, Streamlit

### Autonomous vehicles and simulation

**[NAVIK: Adaptive Path Planning and Collision Avoidance](https://github.com/theflighttechofficial/NAVIK-Simulator)** · Smart India Hackathon 2026 (SIH26037, MathWorks), selected
Team lead for a 6-person team on planning for autonomous vehicles on unstructured Indian roads, where livestock, auto-rickshaws, wrong-way traffic, potholes, and monsoon conditions break lane-based assumptions.
- **Web SIL simulator:** physics engine, trajectory planner, spatial risk field and heat map, traffic agent behavior, telemetry HUD, three camera views, six road scenarios, and Gemini-based reasoning.
- **Planning prototype:** [repo](https://github.com/theflighttechofficial/SIH-2026-Navik-autonomous-Roads). Pins down and validates the planning maths before the MATLAB/Simulink build.
*Stack:* Vanilla JavaScript (ES6+), HTML5 Canvas, SVG, CSS3, Gemini API

### Full-stack and frontend products

**[ResumeForge AI](https://github.com/theflighttechofficial/ResumeForge-AI)** · in development
ATS resume builder and optimizer. Reads a resume the way an ATS and recruiter would, scores it against a job description, and suggests edits. A deterministic checker labels each AI change as supported, inferred, or unsupported, so the tool never invents skills, jobs, or metrics. Moved to an offline-first desktop app with local models through Ollama.
*Stack:* Electron, React, TypeScript, SQLite, Ollama

**[RigForge: PC Hardware Performance Matrix](https://github.com/theflighttechofficial/RigForge)** · in development
PC build simulator. Real-time 3D assembly view with WebGL, Pareto price-to-performance analysis, bottleneck analysis across resolutions, and an AI Build Doctor. Localized for Indian pricing in INR.
*Stack:* React 19, TypeScript, Vite, Three.js, Tailwind CSS, Express, Gemini API

**[FridgeChef AI](https://github.com/theflighttechofficial/FridgeChef-AI)** · in development
Smart fridge and culinary assistant. Ingredient audit from a fridge photo, receipt-to-pantry scanning, zero-waste recipe generation, meal planning, and voice-guided cooking. Per the README, it also targets mobile layouts.
*Stack:* React 19, TypeScript, Vite, Tailwind CSS v4, Express, Gemini API

**[HomeFinder+](https://github.com/theflighttechofficial/Home-Finder-Plus-Rent-Buy-Sell-)**
Rent, buy, and sell listings across India with direct owner contact. Filters for city, budget, property type, bedrooms, furnishing, parking, and amenities. Filters are kept in the URL so searches can be shared. Includes an API reference and test suite.
*Stack:* JavaScript, Tailwind CSS, MongoDB

**[Lumisphere](https://lumisphere-nine.vercel.app)** · [repo](https://github.com/theflighttechofficial/Lumisphere)
Interactive WebGL portfolio. Spring-physics pull-chain lamp, volumetric light shaders, and procedural Web Audio synthesis.
*Stack:* React, Vite, Three.js, framer-motion, GLSL

**[Oru Payanam Aayiram Kathaigal (Tamizh Payanam)](https://github.com/theflighttechofficial/Oru-Payanam-Aayiram-Kathaigal)**
Retro-futuristic web experience on Tamil Nadu culture, music, cinema, and literature, structured as a night government bus journey across six routes. Interactive controls and keyboard shortcuts.
*Stack:* JavaScript, React, Node.js, PostgreSQL

**[Lemuria & Kumari Kandam Explorer](https://github.com/theflighttechofficial/Kumarikandam-the-lost-mythology)**
Interactive research and education app on the Lemuria and Kumari Kandam myths, with historical map exploration and a comparison of myth against oceanographic evidence. Companion to the research paper below.

**[Škoda & Volkswagen Group India Showcase](https://github.com/theflighttechofficial/Skoda-Auto-Volkswagen-India-Pvt-Ltd)**
Single-page buyer's guide covering nine group brands. Dynamic brand themes, powertrain analytics, variant matrix, 360° colour visualizer, configurator, engine sound gallery, and crash-safety deep dive.
*Stack:* JavaScript-based SPA

**[The Wedding Company](https://github.com/theflighttechofficial/The-Wedding-Company)**
Scroll-driven wedding invitation with five-layer parallax, canvas particle systems, a synthesized Web Audio temple bell, RSVP forwarding via WhatsApp or email, and a downloadable calendar (.ics) file. No backend.
*Stack:* React 19, Vite 8, Framer Motion

**[Neoshaan Technologies website](https://github.com/theflighttechofficial/Neoshaan_Technologies)**
Company website from my internship: responsive UI, course catalog, dynamic course pages, contact and application forms.
*Stack:* React, Vite, Node.js, Express

### Research

**[TRUST-TAB / TableAbstain](https://github.com/theflighttechofficial/TRUST-TAB-AI-source-validity-checker)** · in preparation (IEEE format)
Benchmark for whether LLMs abstain when a financial table cannot answer a question. Built from FinQA with five perturbation types, four confidence signals (verbalized confidence, P(True), self-consistency, evidence coverage), and ten evaluation metrics including selective accuracy, AURC, ECE, and Brier score. Runs through Ollama or API clients.
Co-authored with Pradeep Kumar M.
*Stack:* Python, Qwen2.5-7B-Instruct (pilot run)

### Other repositories

- **[Automated PDF-to-Excel Extraction](https://github.com/theflighttechofficial/Automated-PDF-to-excel-data-extraction)**: documentation for the L&T internship project (source confidential).
- **[Scan2Sheet](https://github.com/theflighttechofficial/Scan2Sheet)**: OCR engine for single-line diagram schedules to Excel (L&T internship project, documentation only).
- **[Invisible-cloak](https://github.com/theflighttechofficial/Invisible-cloak)**: real-time OpenCV colour-segmentation invisibility effect, about 30 fps.
- **[Titanic-ML-Project](https://github.com/theflighttechofficial/Titanic-ML-Project)**: Kaggle Titanic survival model, 78.71% accuracy.
- **Lab assignments** for data-structures and algorithms coursework.

**In progress, not yet on GitHub:** FocusBuddy, a Windows desktop companion that detects distracting apps and sites. TrustPulse AI, for the IBM Z Datathon 2026.

---

## Skills

- **Languages:** Python, SQL, TypeScript, JavaScript, C, C++, Java
- **Data and ML:** pandas, NumPy, scikit-learn, XGBoost, SHAP, PyMuPDF, openpyxl, Jupyter
- **Computer vision and OCR:** YOLOv8, OpenCV, Tesseract OCR
- **NLP and LLMs:** RAG, FAISS, BM25, Reciprocal Rank Fusion, SentenceTransformers, GPT-4o, Gemini, Groq, Ollama
- **Frontend:** React, Vite, Tailwind CSS, Zustand, Framer Motion, Three.js, WebGL
- **Backend and data stores:** Node.js, Express, FastAPI, PostgreSQL, MySQL, MongoDB, Supabase, SQLite, Firebase
- **Services and tools:** Razorpay, Resend, Google Calendar API, Vercel, Git, GitHub, Linux, Overleaf / LaTeX

---

## Certifications

- Machine Learning Specialization, Stanford University & DeepLearning.AI (Coursera, Jul 2026)
- Google Data Analytics Professional Certificate (Coursera, Aug 2026)
- Google Prompting Essentials Specialization (Coursera, Jul 2026)
- Microsoft Learn: Creation of ML Models, Build 2026 (Jan 2026)
- HackerRank: SQL Gold, SQL Intermediate, Python Gold, Python Basic (Jul 2026)
- Cisco Networking Academy: Getting Started with Packet Tracer (Aug 2026)
- IBM / Cognitive Class: Python 101 for Data Science (Dec 2025)
- IBM Z Day 2025: AI & Data, IBM Z Skills, Modernization, Security (Dec 2025)

---

## Achievements & Leadership

- **Smart India Hackathon 2026:** selected with NAVIK, team lead.
- **HackerRank Orchestrate (Aug 2026):** MessageMind router, 75% action and 83% type accuracy.
- **Kaggle:** ROGII Wellbore Geology Prediction, public RMSE 136.002. Titanic, 78.71%. AgriYield AI published.
- **SRIHER Research Day 2026:** presented Road-AI.
- **SRIHER Innovation Day:** showcased a cybercrime prevention and active-monitoring software.
- **Academic leadership:** ran an Overleaf / LaTeX seminar for junior students on writing research papers.
- German language learner (A2, working toward B2).

---

## Writing and Profiles

- Blog: [theflighttechlabs.hashnode.dev](https://theflighttechlabs.hashnode.dev). Latest: *How I Automated 3–4 Days of Manual Work at L&T Construction Using Python.*
- Portfolio: [lumisphere-nine.vercel.app](https://lumisphere-nine.vercel.app)
- Kaggle: [kaggle.com/theflighttechofficial](https://kaggle.com/theflighttechofficial)
- HackerRank: [hackerrank.com/profile/umasubramanian81](https://hackerrank.com/profile/umasubramanian81)
- LinkedIn: [linkedin.com/in/varun-vaibhav-s-11b69a2ba](https://linkedin.com/in/varun-vaibhav-s-11b69a2ba)

---

## Let's Connect

Open to data analytics, data engineering, and applied AI roles, and to feedback on my projects.

Email: Umasubramanian81@gmail.com
