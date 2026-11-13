<h1 align="center">Hi, I'm Sumehra Saif 👋</h1>
<h3 align="center">Aspiring AI/ML Engineer & Data Scientist · Computer Science Junior at Boston University · Break Through Tech AI Fellow</h3>

<p align="center">
  <a href="https://www.linkedin.com/in/sumehra-saif"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:sumehra@bu.edu"><img src="https://img.shields.io/badge/BU_Email-CC0000?style=for-the-badge&logo=maildotru&logoColor=white" alt="BU email: sumehra@bu.edu"/></a>
  <a href="mailto:saifsumehra@gmail.com"><img src="https://img.shields.io/badge/Personal_Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Personal email: saifsumehra@gmail.com"/></a>
</p>

---

## 🙋🏻‍♀️ About Me

I'm a junior studying Computer Science at **Boston University** (B.A., expected graduation in May 2028) and an aspiring AI/ML engineer and data scientist/analyst. I build AI systems that hold up in the real world, from voice authentication that catches deepfakes to an LLM copilot that checks software requirements against NASA policy. As a **[Break Through Tech AI/ML Fellow](https://www.breakthroughtech.org/)**, I completed the Summer Machine Learning Foundations Lab and I'm now on a Fall AI Studio team.

- 🔭 **Interested in:** NLP, neural networks, speech & audio ML, data analytics, and AI/ML in healthcare, business and education
- 🛡️ **Building:** [VoiceGuard](https://github.com/sum09fairSaif/voiceguard), voice MFA with anti-spoofing (BU Spark! Product Innovation Fellowship, Fall 2026)
- 🔬 **Seeking research:** research positions and fellowships in AI/ML, NLP, neural networks and data analytics, especially where AI meets healthcare, business or education
- 🎯 **Also seeking:** Summer 2027 internships in AI, ML, data science, data analytics and software engineering
- 🤝 **Ask me about:** being a Break Through Tech fellow, my BU Spark! Product Innovation Fellowship as a Technical Innovator, running Agile sprints as Scrum Master, or tutoring and teaching (CS111 & CS112 Course Assistant and peer tutor in math and CS)

---

## ⭐ Featured Project: [VoiceGuard](https://github.com/sum09fairSaif/voiceguard) · BU Spark! Fellowship

> **Voice-biometric multi-factor authentication that can tell a live speaker from a replay or an AI deepfake.**

One short recording is checked three ways: **what** was said (a prompted passage, not a fixed passphrase), **who** said it (voiceprint match) and **whether** it's a live human (anti-spoofing). All three must pass, and liveness can veto on its own. Raw audio is never stored.

| | |
|---|---|
| **My role** | Technical Innovator, backend owner and Scrum Master on a 4-person team, working with 5 technical mentors |
| **What I built** | The FastAPI backend (auth with lockout, single-use challenge passages, the three-check verification pipeline, Fernet-encrypted voiceprints), the PyTorch model service on Hugging Face Spaces, the AASIST liveness fine-tuning and evaluation pipeline across ASVspoof, In-the-Wild and CodecFake data, and GitHub Actions CI. I also lead UI/UX planning with our frontend developer and review all frontend code. |
| **Tools** | Python · FastAPI · PyTorch · SpeechBrain (ECAPA) · AASIST · OpenAI Whisper · MongoDB Atlas · React + TypeScript · Vercel · Render |
| **Result** | Deployed end to end: [live app](https://voiceguard-nu.vercel.app/) and [API docs](https://voiceguard-83cj.onrender.com/docs) |

👉 **[Read the full project README](https://github.com/sum09fairSaif/voiceguard)**

---

## ⭐ Featured Project: [AI Compliance Copilot](https://github.com/Break-Through-Tech/Aerospace-1A-compliance-copilot) · Break Through Tech AI Studio

> **An AI first-pass auditor that checks a Software Requirements Specification against NASA's software engineering standard (NPR 7150.2D) and returns cited, verifiable findings.**

| | |
|---|---|
| **What we built** | An 8-person team extracted 100 requirement clauses from the NASA standard, built a TF-IDF and keyword-rule baseline, then a RAG pipeline. It retrieves the relevant NASA clauses for each requirement and has an LLM return a schema-validated verdict (compliant, partial, non-compliant or unclear) that must cite at least one clause. |
| **My contribution** | **Data (Sep):** helped source the NASA standard and build the 100-clause dataset (pdfplumber + regex extraction joined to the Appendix C compliance matrix). I tagged each clause with a functional category and the actions it requires, and wrote the team's first analysis of the SRS we audit.<br>**RAG pipeline (Oct):** integrated the RAG baseline end to end. For each of the 54 requirements it retrieves the top 3 NASA clauses and calls `gpt-4o-mini` with structured outputs. I designed the Pydantic schemas (`DocumentMatch`, `CitedSource`, `RAGResponseSchema`) that force every verdict to cite NASA clauses with exact quotes, and fixed the clause-ID mismatches that blocked validation. I got the full 54-requirement run to complete by switching from Gemini to OpenAI when Gemini kept failing under load.<br>**Project management (ongoing):** I keep the team's product backlog and create, set up and maintain the GitHub issues and Project board for all 8 members. I also wrote the project README. |
| **Tools** | Python · pdfplumber · pandas · scikit-learn (TF-IDF) · ChromaDB · Qwen3-Embedding · OpenAI API (structured outputs) · Groq · Pydantic · pytest · Google Colab |
| **Status** | Baseline and RAG pipeline done; tool-calling agent and benchmark evaluation in progress (Fall 2026) |

👉 **[Project repo](https://github.com/Break-Through-Tech/Aerospace-1A-compliance-copilot)**

---

## 🚀 More Projects

| Project | What it does | Built with |
|---|---|---|
| **[BananaVision](https://github.com/sum09fairSaif/BananaVision)** · Coding It Forward | Mobile app that predicts a banana's ripeness, shelf life in days and nutrient profile from one photo. I trained a MobileNetV2 transfer-learning model and shipped it as quantized TensorFlow Lite. | TensorFlow Lite · FastAPI · React Native (Expo) · Render |
| **[Student Dropout Prediction](https://github.com/sum09fairSaif/iX_Class-Final-Project_Academic-Success-and-Dropout)** · iX class final project | Predicts whether a student will drop out, stay enrolled or graduate (4,424 students), so schools can flag at-risk students after the first semester. A tuned Random Forest reached 77.9% accuracy (0.80 dropout F1). The analysis found that students behind on tuition dropped out at 86.6% vs. 24.7% for those who were current. | Python · pandas · scikit-learn · Matplotlib · Seaborn |
| **[FrontHealth](https://github.com/sum09fairSaif/Front-Health)** · MIT GenAI Hackathon 2026 | Tracks each cancer patient's path from diagnostic referral to test completion and follow-up, with clinician and patient apps and FHIR-based data exchange. | TypeScript · PostgreSQL · Redis · Kafka · Docker · Kubernetes |
| **[connectHer](https://github.com/sum09fairSaif/connecther)** · HackBeanPot 2026 | AI-powered prenatal fitness platform with symptom-aware workout recommendations from Gemini, and voice navigation for multilingual access. | React · TypeScript · Node.js/Express · Supabase · Auth0 · Gemini API |
| **[Text Similarity Classifier](https://github.com/sum09fairSaif/Text-Similarity-Classifier)** · BU CS111 | Identifies which known author or source an unknown text most likely came from. It compares five statistical features (word, stem, word-length, sentence-length and vowel frequencies) using log-likelihood scoring, all built from scratch, including a custom stemmer. | Python (no NLP libraries) |
| **[Tic-Tac-Toe with Minimax AI](https://github.com/sum09fairSaif/Tic-Tac-Toe-Java-)** | Terminal game with an unbeatable AI opponent that uses the Minimax algorithm, plus one- and two-player modes, input validation and a CSV-backed leaderboard. | Java |

---

## 🛠 Tech Stack
<!-- Keep only what you can talk about in an interview. Badges come from https://shields.io and https://simpleicons.org. -->

**Languages**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)

**ML, AI & Data**
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow_Lite-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=flat-square&logo=scipy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat-square&logo=python&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=flat-square&logo=python&logoColor=white)
![spaCy](https://img.shields.io/badge/spaCy-09A3D5?style=flat-square&logo=spacy&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging_Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![SpeechBrain](https://img.shields.io/badge/SpeechBrain-4B8BBE?style=flat-square&logo=python&logoColor=white)
![OpenAI Whisper](https://img.shields.io/badge/Whisper-412991?style=flat-square&logo=openai&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6446?style=flat-square&logo=python&logoColor=white)
![Pydantic](https://img.shields.io/badge/Pydantic-E92063?style=flat-square&logo=pydantic&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)

**Backend & Web**
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white)

**Data, Cloud & DevOps**
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)
![Render](https://img.shields.io/badge/Render-46E3B7?style=flat-square&logo=render&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

---

## 🌱 Currently Learning
<!-- Anything here is fair game in an interview. -->
- Retrieval-augmented generation and tool-calling LLM agents (AI Studio), and LangGraph for agentic workflows
- Speech anti-spoofing: fine-tuning and evaluating deepfake-voice detectors (VoiceGuard)

---

## 🏆 Fellowships & Certifications
- 🎓 **Summer Machine Learning Foundations Lab**, Break Through Tech AI Program · Summer 2026 · [View credential](https://mycredentials.ecornell.cornell.edu/credential/BwRfqdRQcI)
- 🤖 **Break Through Tech AI/ML Fellow**, selected from 4,000+ applicants nationwide · 2026–present
- 🚀 **BU Spark! Product Innovation Fellow** (XC 475) · Fall 2026
- 🧠 **[Technical AI Safety Fellow](https://buaisa.org/programs/technical)**, AI Safety & Alignment at BU (AISA) · Fall 2026–present: an 8-week program on RLHF, mechanistic interpretability, model evaluations, red-teaming and scalable oversight
- 🇺🇸 **Coding It Forward Fellow** · Summer 2026
- ⚡ **Hackathons:** MIT GenAI Hackathon 2026 (FrontHealth), HackBeanPot 2026 (connectHer)

---

## 💡 Beyond the Code
- 🔐 **Co-President**, BU Women in CyberSecurity (WiCyS) Student Chapter · Feb–Aug 2026. Before that I was Vice President (May 2025–Feb 2026) and Social Media Chair (Oct 2024–Apr 2025).
- 👥 **Clubs:** BU Girls Who Code, BU Hack4Impact, BU AI/ML Society
- 🧑‍🏫 **Course Assistant**, BU Computer Science. **CS112** (Java & OOP, Aug 2026–present): I support ~150 students. **CS111** (Python & digital logic, Sep–Dec 2025): I helped in weekly labs of ~30 and held office hours for a 300+ student course. In both I grade coding assignments, quizzes and labs with personalized feedback on code quality, style and efficiency.
- 🎒 **Orientation Leader** (Jul 2025–Jan 2026) and **Program Assistant, Summer Challenge** (Jun–Aug 2026), Boston University
- ➗ **Peer Tutor**, BU Educational Resource Center (ERC): Calculus I, Calculus II, Linear Algebra and Introduction to Computer Science I (Python)
- 🌏 **Teacher Intern**, Grameen Shikkha & Dream Hope School, Dhaka, Bangladesh · Dec 2024–Jan 2025: I taught English and math to 20–25 underprivileged 5th graders, and computer literacy and graphic design to 15–20 high school students
- 🔁 **Scrum Master** for the VoiceGuard team: I run sprint planning, stand-ups, reviews and retros
- 💃 **Off the clock:** dancing, music, K-dramas, travel, trying new cuisines, and cafe-hopping with friends on a hunt for the best matcha 🍵

---

## 📊 GitHub Stats
<p align="center">
  <img height="180" src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=sum09fairSaif&theme=github" alt="GitHub stats"/>
  <img height="180" src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=sum09fairSaif&theme=github" alt="Top languages"/>
</p>
<p align="center">
  <img src="https://streak-stats.demolab.com?user=sum09fairSaif&hide_border=true" alt="GitHub streak"/>
</p>
