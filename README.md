# Hardik Thapar

**Backend & ML · B.E. Computer Science, Chitkara University (2028) · Open to Software Engineering internships, Summer 2027**

Third-year Computer Science student in Chandigarh, India. I build backend systems and the data pipelines behind ML work, and I test what they do under load, during a crash, and on the retry.

---

## Selected Projects

### [Dispatch](https://github.com/hardik-thapar/dispatch) · Go, PostgreSQL
A fault-tolerant job queue built on PostgreSQL.

- Workers claim jobs with `FOR UPDATE SKIP LOCKED`, hold leases kept alive by heartbeats, and are fenced by attempt number. Failed jobs retry with exponential backoff and jitter, then go to a dead-letter queue with replay. Submits are idempotent.
- A chaos harness `kill -9`s workers under load: across 6,000 jobs and 60 crashes, **0 jobs lost** and **0 duplicate effects** from the idempotent handler (a non-idempotent control produced 120).
- `SKIP LOCKED` gave 0 double claims vs 102,921 for select-then-update. A partial index cut the claim query from 60.7 ms to 0.006 ms on 1,000,000 rows.
- About 4,600 jobs/s peak with no-op jobs (16 workers, one laptop); p99 queue wait of 18 ms or less at 500–2,000 jobs/s.
- `make bench` and `make chaos` reproduce every number. Methods and raw output are in [RESULTS.md](https://github.com/hardik-thapar/dispatch/blob/main/RESULTS.md); bugs found along the way are written up in `BUGS.md`.

### [VocalWell](https://github.com/hardik-thapar/vocalwell_backend) · Python, FastAPI, PostgreSQL
A containerized backend for voice-pathology screening: it takes a voice recording and returns a class (Healthy, Laryngitis or Vocal Polyp), a risk level and a multi-page PDF report.

- I wrote the backend: the FastAPI service, Librosa feature extraction, PostgreSQL storage (raw SQL over SQLAlchemy connection pooling), ReportLab reports, the Docker Compose setup and an integration test script.
- It serves a pre-trained TensorFlow CNN built by my teammates.

### [DengCast](https://github.com/hardik-thapar/dengcast-dengue-forecasting) · Python, CatBoost
Weekly dengue case forecasting on the DrivenData DengAI benchmark.

- Lag features, rolling statistics, a log-transformed target, and chronological cross-validation to avoid leakage.
- MAE **11.87** (San Juan) and **4.74** (Iquitos), against baselines of about 30 and 31.

### [EEG Alzheimer's Detection](https://github.com/hardik-thapar/eeg-alzheimer-detection) · Python
Alzheimer's detection from 19-channel resting-state EEG under strict leave-one-subject-out evaluation. The lab's results show that epoch-level evaluation inflates accuracy by about 9.4 percentage points.

---

## Experience

**Research Intern, Software & Data Systems** · National Kaohsiung University of Science and Technology (NKUST), Taiwan · Remote · Mar–May 2026

Under Assoc. Prof. Chang Kang-Ming. Built the Python preprocessing and feature-extraction pipelines for 19-channel EEG (OpenNeuro ds004504, 65 subjects) and ran the lab's experiments through them. Worked with the professor and PhD students on a hybrid EEG model.

---

## What I Work With

**Languages** &nbsp; `Go` `Java` `Python` `SQL` `JavaScript`

**Backend** &nbsp; `REST APIs` `Gin` `FastAPI` `PostgreSQL` `SQLAlchemy`

**Testing** &nbsp; `testcontainers-go` `Go race detector` `Chaos testing` `Integration testing`

**ML** &nbsp; `scikit-learn` `CatBoost` `pandas` `NumPy` `Librosa` `Time-series forecasting`

**Tools & Cloud** &nbsp; `Docker` `Docker Compose` `Git` `Linux` `AWS (SageMaker · Bedrock)`

---

## Recognition

- **1st place**: Swasthathon 2025 (PCI India, 436 teams) and HackEMinds 2025
- **Winner**: CodePi 2025 (global, 600+ participants), GDG North India, Code With DCG (DTU); EduChain track winner at Hackaccino 3.0 (300+ teams)
- **Runner-up**: Hackfest 2.0 (GDG Cloud New Delhi) and HackWithHer 4.0 (IEEE)
- **National finalist**: AMD AI Sprint, IIT Bombay (top 150 of 4,000) and GSMA Network-as-Code Hackathon, IMC 2025 (top 50 of 2,000)
- AWS AI & ML Scholar 2025 · McKinsey Forward Program 2025–26 · Harvard Aspire Leaders Program 2025
- 250+ problems on [LeetCode](https://leetcode.com/u/HARDIKTHAPAR/), mostly in Java

---

## Get In Touch

[Portfolio](https://hardik-thapar.github.io) · [LinkedIn](https://linkedin.com/in/hardik-thapar) · [X](https://x.com/ThaparHardik) · hardikthapar1@gmail.com
