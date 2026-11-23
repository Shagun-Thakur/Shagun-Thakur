<!--
  PROFILE README: Shagun Thakur
  Palette: navy #0A1426 · steel #2F6FAE · silver #C9D6E3 · accent cyan #6CC4E8
  Place this file and the assets/ folder at the root of your <username>/<username> repo.
-->

<div align="center">
  <img src="assets/header.svg" width="100%" alt="Shagun Thakur: Machine Learning, Audio AI, Intelligent Systems" />
  <br/>
  <a href="https://www.linkedin.com/in/shagun-thakur-8509b7281"><img src="https://img.shields.io/badge/LinkedIn-14284B?style=flat-square&logoColor=white&logo=linkedin" alt="LinkedIn" /></a>
  <a href="mailto:thakurshagun412@gmail.com"><img src="https://img.shields.io/badge/Email-14284B?style=flat-square&logoColor=white&logo=gmail" alt="Email" /></a>
  <a href="https://auralq-r77uc2bkz7wgu7yifqkduu.streamlit.app/"><img src="https://img.shields.io/badge/AuralQ%20Live%20Demo-2F6FAE?style=flat-square&logoColor=white" alt="AuralQ Live Demo" /></a>
  <a href="https://glycoscan-k7jecpfxz98wveubzmfayp.streamlit.app/"><img src="https://img.shields.io/badge/GlycoScan%20Live%20Demo-2F6FAE?style=flat-square&logoColor=white" alt="GlycoScan Live Demo" /></a>
</div>

## About

Final-year Computer Science undergraduate focused on applied machine learning for real-world physical and sensor signals—especially audio, acoustics, and vibration. I build verifiable systems pairing machine learning with deterministic signal processing, multi-seed statistical evaluation, and edge deployment under strict compute budgets (such as 4 GB consumer GPUs).

**Open to:** research internships (Jan–Jun 2027) and ML/AI roles at startups, including new domains where the problem is hard.

## Flagship Projects

<a href="https://github.com/Shagun-Thakur/AuralQ"><img src="assets/card-auralq.svg" width="100%" alt="AuralQ" /></a>

<!-- Visual Proof Placeholder: 10-second screen recording / GIF of AuralQ answering an acoustic question with verified citation chips (e.g. assets/auralq-demo.gif) -->

- **Problem:** Multimodal audio LLMs hallucinate acoustic measurements, fail on exact numeric queries, and rely on cloud APIs that compromise data privacy.
- **Approach:** Pairs a quantized local LLM (Ollama, `llama3.2:3b`) strictly for intent parsing with 8 closed-form DSP tools (`librosa`/`scipy`) and an independent regex citation guardrail (±5% tolerance).
- **Results:** Achieves 99.0% citation grounding (vs. 90.0% LLM-only) and 100% abstention on out-of-scope audio; runs air-gapped on a 4 GB RTX 3050 (<2.4 GB peak VRAM, <6.7s latency) with 74 passing tests.

<details>
<summary><b>Benchmark results (AuralQ vs. Baselines)</b></summary>
<br/>

| Metric (20-case benchmark) | LLM only (B2) | Fixed pipeline (B3) | **AuralQ (B4)** |
|---|:---:|:---:|:---:|
| Citation grounding rate | 90.0% | 94.4% | **99.0%** |
| Numeric hallucination rate | 10.0% | 10.0% | **5.0%** |
| Abstention accuracy | 90.0% | 90.0% | **100.0%** |

*Note: 20-case benchmark — indicates practical performance differences, not statistical significance.*

</details>

[Repository](https://github.com/Shagun-Thakur/AuralQ) · [Live Demo](https://auralq-r77uc2bkz7wgu7yifqkduu.streamlit.app/)

<br/>

<a href="https://github.com/Shagun-Thakur/EchoGuard"><img src="assets/card-echoguard.svg" width="100%" alt="EchoGuard" /></a>

- **Problem:** Industrial anomaly detection often relies on raw high-dimensional spectrograms, which are computationally expensive and prone to overfitting without labeled defect data.
- **Approach:** Combines a 6-method feature selection pipeline (ANOVA, mutual information, RF importance, PCA/t-SNE) to distill 50 acoustic descriptors into 9 interpretable features on the MIMII pump dataset (`id_00`, ch0).
- **Results:** Cut training time 25× (~25 min to ~1 min) while boosting Autoencoder ROC-AUC from 72.23% to 96.93%; Normalizing Flows reached 98.34 ± 0.76% ROC-AUC across 10 random seeds.

[Repository](https://github.com/Shagun-Thakur/EchoGuard) · [Live Demo](https://echoguard-etbpz3hmxxfke7mxfpgdt7.streamlit.app/)

<br/>

<a href="https://github.com/Shagun-Thakur/smart-home-openenv"><img src="assets/card-smarthome.svg" width="100%" alt="Smart Home OpenEnv" /></a>

- **Problem:** Reinforcement learning benchmarks for residential energy management often lack reproducibility, realistic physics, and rigorous baseline comparisons.
- **Approach:** Built a custom Gymnasium environment modeling HVAC and battery storage dynamics under time-of-use tariffs, thermal inertia, and Markov occupancy.
- **Results:** Evaluated over 10 training and 50 disjoint test seeds; showed PPO beats heuristic rules but is statistically tied with a constant 24°C baseline ($p = 0.789$). Backed by 38 tests, containerized on Hugging Face Spaces via FastAPI/Docker.

[Repository](https://github.com/Shagun-Thakur/smart-home-openenv)

## Collaboration & Open Source

<a href="https://github.com/AnonAjay/Titans-Arcade"><img src="assets/card-titans.svg" width="100%" alt="Titans Arcade" /></a>

<!-- Visual Proof Placeholder: 5-second GIF of live 60 FPS gameplay / venue calibration UI (e.g. assets/titans-demo.gif) -->

Architected the computer vision and kinematics pipeline for an offline physical arcade running on standard laptop webcams at 60 FPS without depth sensors (awarded **1st Place at Tech-Fest**). Mapped camera pixels to physical floor coordinates using planar homography with a ground-plane constraint, built scale-invariant joint angle posture matching, and decoupled neural inference into background threads to guarantee a smooth 60 FPS render loop under live crowd conditions.

[Repository](https://github.com/AnonAjay/Titans-Arcade)

<br/>

<a href="https://github.com/Anjalisahni24/ResQ_Audio_ANNapp"><img src="assets/card-resq.svg" width="100%" alt="ResQ" /></a>

Engineered and trained the core acoustic detection model for emergency sound classification (distress calls, impacts) integrated into an active Android safety app.

[Repository](https://github.com/Anjalisahni24/ResQ_Audio_ANNapp)

<br/>

<a href="https://github.com/AnonAjay/Jaanch"><img src="assets/card-jaanch.svg" width="100%" alt="Jaanch" /></a>

Resolved cross-origin iframe microphone permissions and fixed real-time audio stream bugs across the browser speech-to-text (STT) and text-to-speech (TTS) pipeline.

[Repository](https://github.com/AnonAjay/Jaanch)

## Also Built

<details>
<summary><b>Other projects (Tabular ML, Speech, IoT)</b></summary>
<br/>

- [**GlycoScan**](https://github.com/Shagun-Thakur/GlycoScan) ([Live Demo](https://glycoscan-k7jecpfxz98wveubzmfayp.streamlit.app/)): Interactive clinical range checker and Random Forest risk model on the Pima Indians diabetes dataset.
- [**Customer Churn Platform**](https://github.com/Shagun-Thakur/Customer-churn-prediction): Churn prediction pipeline comparing XGBoost and Random Forest with feature importance explanations in Streamlit.
- [**Multi-Sensor IoT Monitoring**](https://github.com/Shagun-Thakur/Multi--Sensor-IoT-ML-Industrial-Monitoring-System): Anomaly detection and degradation tracking pipeline across simulated sensor streams.
- [**AI Voice Assistant**](https://github.com/Shagun-Thakur/AI_Voice_Assistant): Multilingual speech-to-speech pipeline with intent parsing.

</details>

## Technical Toolkit

| Level | Tools & Frameworks |
|---|---|
| **Core strengths** | **Python**, **PyTorch**, **Librosa**, **SciPy**, **scikit-learn**, **FastAPI**, **Docker**, **Streamlit**, **pytest**, **Local LLMs (Ollama)** |
| **Used in specific projects** | OpenCV, MediaPipe *(Titans Arcade)* · Gymnasium, Stable-Baselines3 *(Smart Home OpenEnv)* · TensorFlow · XGBoost · C++ |

## Let's Connect

Open to discussing research internships (Jan–Jun 2027), startup engineering roles, Audio AI, and verifiable ML systems.

[LinkedIn](https://www.linkedin.com/in/shagun-thakur-8509b7281) · [Email](mailto:thakurshagun412@gmail.com) · [GitHub](https://github.com/Shagun-Thakur)
