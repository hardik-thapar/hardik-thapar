# Hardik Thapar

**Backend & ML · B.E. Computer Science, Chitkara University (2028) · Open to Software Engineering internships, Summer 2027**

Third-year Computer Science student in Chandigarh, India. I build backend systems and the data pipelines behind ML work, and I test what they do under load, during a crash, and on the retry.

[Portfolio](https://hardik-thapar.github.io) · [LinkedIn](https://linkedin.com/in/hardik-thapar) · [LeetCode](https://leetcode.com/u/HARDIKTHAPAR/) · hardikthapar1@gmail.com

---

## Projects

**[Dispatch](https://github.com/hardik-thapar/dispatch)**  
`Go` `PostgreSQL` `Docker`  
A crash-safe job queue: workers claim jobs with `SKIP LOCKED` and hold heartbeat leases, and attempt-number fencing stops a stale worker from finishing a job it has lost. Chaos test: workers killed 60 times across 6,000 jobs, **0 lost, 0 duplicate effects**, reproducible with `make chaos`.

**[VocalWell](https://github.com/hardik-thapar/vocalwell_backend)**  
`FastAPI` `PostgreSQL` `Docker Compose`  
A voice recording goes in; a classification, a risk level and a PDF report come out. I built the backend (Librosa features, PostgreSQL storage, ReportLab reports, integration tests); the CNN it serves is my teammates'.

**[DengCast](https://github.com/hardik-thapar/dengcast-dengue-forecasting)**  
`Python` `CatBoost` `pandas`  
Weekly dengue forecasts on the DengAI benchmark, with lag features and chronological cross-validation so no future data leaks into training. MAE **11.87** and **4.74** against baselines of about 30 and 31.

**[EEG Alzheimer's Detection](https://github.com/hardik-thapar/eeg-alzheimer-detection)**  
`Python`  
Alzheimer's detection from 19-channel EEG, evaluated leave-one-subject-out so no person is in both training and test. The lab's results show that splitting by epoch instead inflates accuracy by about 9.4 points.

---

## Experience

**Research Intern, Software & Data Systems** · NKUST, Taiwan · Remote · Mar–May 2026  
Built the Python preprocessing and feature-extraction pipelines for 19-channel EEG (OpenNeuro ds004504, 65 subjects) under Assoc. Prof. Chang Kang-Ming, and ran the lab's experiments through them.

---

## Recognition

- **1st place**: Swasthathon 2025 (PCI India, 436 teams) and HackEMinds 2025
- **Winner**: CodePi 2025 (global, 600+ participants), GDG North India, Code With DCG (DTU); EduChain track winner at Hackaccino 3.0
- **Runner-up**: Hackfest 2.0 (GDG Cloud New Delhi) and HackWithHer 4.0 (IEEE)
- **National finalist**: AMD AI Sprint, IIT Bombay (top 150 of 4,000) and GSMA Network-as-Code Hackathon, IMC 2025 (top 50 of 2,000)
- AWS AI & ML Scholar 2025 · McKinsey Forward Program 2025–26 · Harvard Aspire Leaders Program 2025
- 250+ LeetCode problems, mostly in Java

---

## Tech

**Languages** &nbsp; `Go` `Java` `Python` `SQL` `JavaScript`  
**Backend & Data** &nbsp; `REST APIs` `Gin` `FastAPI` `PostgreSQL` `SQLAlchemy`  
**Testing** &nbsp; `testcontainers-go` `Go race detector` `Chaos testing`  
**ML** &nbsp; `scikit-learn` `CatBoost` `pandas` `NumPy` `Librosa`  
**Tools & Cloud** &nbsp; `Docker` `Git` `Linux` `AWS (SageMaker · Bedrock)`
