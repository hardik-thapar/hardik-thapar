# Hardik Thapar

**Software Engineer · Backend & ML · Open to Software Engineering Internships (Summer 2027)**

Third-year Computer Science student at Chitkara University, India. I build backend systems and the data pipelines behind ML work, and I care about what they do under load, during a crash, and on the retry. 

---

## What I Work With

**Languages**  
`Go` `Java` `Python` `SQL` `C++`

**Backend**  
`REST APIs` `Gin` `FastAPI` `PostgreSQL` `SQLAlchemy` `Concurrency` `Idempotency` `Fault tolerance`

**Engineering**  
`Docker` `Docker Compose` `Git` `Linux` `testcontainers-go` `Integration testing`

**ML**  
`TensorFlow / Keras` `scikit-learn` `CatBoost` `Librosa` `Time-series forecasting` `Feature engineering`

**Cloud**  
`AWS (SageMaker · Bedrock)`

---

## Selected Projects

**[Dispatch](https://github.com/hardik-thapar/dispatch)** — Fault-tolerant job queue on PostgreSQL, written in Go. `FOR UPDATE SKIP LOCKED` claims, leases with heartbeats, attempt-number fencing, exponential backoff with jitter, dead-lettering with replay, idempotent submit. A chaos harness `kill -9`s workers under load: across 6,000 jobs and 60 crashes, 0 jobs lost and 0 duplicate effects from the idempotent handler. About 4,600 jobs/s peak at 16 workers, p99 queue wait of 18 ms or less. Methods and raw output in [RESULTS.md](https://github.com/hardik-thapar/dispatch/blob/main/RESULTS.md).

**[VocalWell](https://github.com/hardik-thapar/vocalwell_backend)** — Containerized FastAPI backend for voice-pathology screening. Librosa feature extraction, a TensorFlow CNN for three-class classification, multi-page PDF reports with ReportLab, PostgreSQL storage, Docker Compose, and an integration test script.

**[DengCast](https://github.com/hardik-thapar/dengcast-dengue-forecasting)** — Weekly dengue case forecasting on the DrivenData DengAI benchmark. Lag features, rolling statistics, a log-transformed target and chronological cross-validation to avoid leakage. MAE 11.87 (San Juan) and 4.74 (Iquitos) against baselines of about 30.

**[EEG Alzheimer's Detection](https://github.com/hardik-thapar/eeg-alzheimer-detection)** — Alzheimer's detection from 19-channel resting-state EEG under strict leave-one-subject-out evaluation. The lab's results show epoch-level evaluation inflates accuracy by about 9.4 percentage points.

---

## Research

**National Kaohsiung University of Science and Technology (NKUST), Taiwan** — Research Intern, Software & Data Systems, March to May 2026, under **Assoc. Prof. Chang Kang-Ming**. Built the Python preprocessing and feature-extraction pipelines for 19-channel EEG (OpenNeuro ds004504, 65 subjects) and ran the lab's experiments through them; took part in designing a hybrid EEG model with the professor and PhD students.

---

## A Few Things

- 1st place at **Swasthathon 2025** (PCI India, 436 teams), **Hackaccino 3.0** (300+ teams) and **HackEMinds 2025**; 8 hackathon wins in total
- National finalist at **AMD AI Sprint, IIT Bombay** (top 150 of 4,000) and **GSMA Network-as-Code Hackathon, IMC 2025** (top 50 of 2,000)
- AWS AI & ML Scholar 2025, McKinsey Forward Program 2025–26, Harvard Aspire Leaders Program 2025
- 250+ problems on [LeetCode](https://leetcode.com/u/HARDIKTHAPAR/), mostly Java

---

## Get In Touch

[Portfolio](https://hardik-thapar.github.io) · [LinkedIn](https://linkedin.com/in/hardik-thapar) · [X](https://x.com/ThaparHardik) · hardikthapar1@gmail.com
