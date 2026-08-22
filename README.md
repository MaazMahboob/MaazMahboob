<p align="center">
  <img src="assets/hero.svg" width="100%" alt="Maaz Mahboob — computer vision and medical AI">
</p>

<p align="center">
  <sub>B.Tech AI, Zakir Husain College of Engineering &amp; Technology, AMU &middot; GATE 2025, Data Science &amp; AI &middot; IELTS 7.0 (C1)</sub>
</p>

I work on computer vision and applied NLP, mostly in healthcare settings where a wrong answer costs more than a wrong guess usually does. Most of what's below started as coursework or an internship and turned into something I kept building on afterward.

### Focus areas

- **Vision** — PyTorch, YOLO (v11 / v12), Faster R-CNN, OpenCV
- **Language & retrieval** — LangGraph, RAG pipelines, PubMedBERT
- **Systems** — FastAPI, Streamlit, SQLite, PostgreSQL

### Research

<details>
<summary><strong>Three papers, at different stages</strong></summary>
<br>

**AI-Driven Multi-Disease Diagnosis Using Medical Imaging for Rural Healthcare**
Book chapter, IGI Global. A YOLOv11 / Faster R-CNN system for localizing 14 thoracic abnormalities in chest X-rays, aimed at resource-constrained healthcare settings. With F. Khan, M. Imran, T. Jamal.

**Symptoms-Based Disease Prediction and Recommendation System Using NLP Query and PubMed BERT**
International Journal of Information Technology, Springer — under review. A fine-tuned PubMedBERT pipeline reaching 94.6% test accuracy across 41 disease classes. Authors: S. S. Ali, M. F. Siddiqui, A. Khan, **M. Mahboob**, S. Ansari.

**Mitigating LLM Hallucinations through Domain-Grounded Tiered Retrieval**
arXiv, 2026. A four-phase LangGraph RAG pipeline with atomic claim verification, evaluated on TimeQA v2 (83.7% win rate) and MMLU Global Facts (78.0%) across 650 queries. Authors: Md. A. Haque, A. Mehdi, T. Fatima, **M. Mahboob**.

</details>

### Projects

<details>
<summary><strong>Chest X-ray abnormality detection</strong></summary>
<br>

Two related builds, kept separate here because they used different models and different codebases:

**B.Tech thesis** (Sep 2024 – May 2025) — fine-tuned YOLOv11 and Faster R-CNN (via Detectron2) on 15,000 chest X-rays across 15 abnormality classes plus "No Finding" (VinBigData), improving mAP@0.5 by 30% over baseline through augmentation and class-rebalancing.

**Deployed app, SURE ProEd capstone** (Sep 2025 – Mar 2026) — a single-file Streamlit application (~2,400 lines) running YOLOv12-m on ChestX-ray14 (14 classes), with role-based access for doctors, admins and patients, SQLite storage, Ollama-generated clinical impressions, PDF reports via FPDF, and a retraining loop where physician-corrected findings become new YOLO training labels.

</details>

<details>
<summary><strong>Other builds</strong></summary>
<br>

**Sign language recognition** — LSTM and GRU models on MediaPipe Holistic landmarks, classifying 50 ASL gestures. 99% (LSTM) and 98% (GRU) accuracy at 15-frame inputs; at 26 frames the LSTM accuracy collapsed to 1.25% while the GRU held at 98.6% — a reminder that a strong short-sequence number doesn't always survive longer inputs.

**Stroke-risk prediction, GNCIPL** — CTGAN-generated minority samples on a 19.5:1 imbalanced clinical dataset, benchmarking XGBoost, Random Forest and Logistic Regression, with holdout testing that surfaced a real gap between synthetic and real-data generalization.

**Loan approval & churn models, GNCIPL** — a Deep ANN for loan approval (92.3% accuracy) and a Random Forest churn model (86.4% accuracy), using dropout, batch normalization, RFM features and K-Means clustering.

**Used car price prediction** — a Scikit-learn regression pipeline reaching 96.9% test performance after cross-validation and hyperparameter tuning.

</details>

### Experience

<details>
<summary><strong>Internships and leadership</strong></summary>
<br>

- **SURE ProEd** (formerly SURE Trust) — Python & ML Intern, G36 batch, remote, Sep 2025 – Mar 2026. Mentor: Bhargavesh Dakka.
- **GNCIPL** — AI/ML Intern, Greater Noida, Oct – Dec 2025.
- **Kodacy** — remote, Jun – Jul 2025.
- **AMU Machine Learning Club** — Publicity Executive, Mar 2023 – Aug 2024. Led a 10-member outreach team across 5+ workshops, bootcamps and hackathons reaching 200+ students; event participation grew 50%, club membership grew 40%.

</details>

<br>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=MaazMahboob&show_icons=true&hide_border=true&bg_color=16130F&title_color=EDE6D9&text_color=9E9484&icon_color=C98A4B" height="165" alt="GitHub stats"/>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/MaazMahboob/MaazMahboob/output/github-contribution-grid-snake-dark.svg" width="100%" alt="Contribution snake"/>
</p>

<p align="center">
  <sub>you@example.com &middot; linkedin.com/in/your-handle — replace with your real links before pushing</sub>
</p>
