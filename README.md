<!--
  PROFILE README: Shagun Thakur
  Palette: navy #0A1426 · steel #2F6FAE · silver #C9D6E3 · accent cyan #6CC4E8
  Place this file and the assets/ folder at the root of your <username>/<username> repo.
-->

<div align="center">
  <img src="assets/header.svg" width="100%" alt="Shagun Thakur: Machine Learning, Audio AI, Intelligent Systems" />
  <br/>
  <a href="https://www.linkedin.com/in/shagun-thakur-8509b7281"><img src="https://img.shields.io/badge/LinkedIn-14284B?style=flat-square&logoColor=white&logo=linkedin" alt="LinkedIn" /></a>
  <a href="mailto:12shagun2005@gmail.com"><img src="https://img.shields.io/badge/Email-14284B?style=flat-square&logoColor=white&logo=gmail" alt="Email" /></a>
  <a href="https://auralq-r77uc2bkz7wgu7yifqkduu.streamlit.app/"><img src="https://img.shields.io/badge/AuralQ%20Live%20Demo-2F6FAE?style=flat-square&logoColor=white" alt="AuralQ Live Demo" /></a>
  <a href="https://glycoscan-k7jecpfxz98wveubzmfayp.streamlit.app/"><img src="https://img.shields.io/badge/GlycoScan%20Live%20Demo-2F6FAE?style=flat-square&logoColor=white" alt="GlycoScan Live Demo" /></a>
</div>

## About

I'm a Computer Science undergraduate interested in how machines learn from **real-world physical signals**: acoustic waves, vibrations, and sensory time series.

My work spans **Machine Learning, Deep Learning, Audio Signal Processing, and Deterministic AI Grounding**. I focus on pairing closed-form signal mathematics with modern learning architectures to build **verifiable, hallucination-resistant systems** that run efficiently on accessible hardware.

## Current Research

How do signal representations, learning methods, and deterministic guardrails interact to make ML systems reliable in real sensory environments?

- **Audio AI & acoustic grounding:** eliminating acoustic hallucinations by pairing local LLMs with closed-form DSP algorithms behind strict citation guardrails.
- **Unsupervised anomaly detection:** representation learning, generative modeling, and multi-method feature extraction on complex industrial soundscapes.
- **Resource-constrained AI:** high-efficiency architectures that run locally on consumer-grade hardware (sub-4 GB VRAM).

### Field research: Project Tarini (precipitation nowcasting)

In flood-vulnerable regions such as the Brahmaputra basin in Assam, extreme monsoon downpours and sudden cloudbursts can trigger catastrophic flash floods within hours, putting communities, agriculture, and infrastructure at severe risk.

Traditional numerical weather forecasting often lacks the rapid, localized granularity that emergency response requires. **Project Tarini** is an ongoing research initiative investigating spatio-temporal precipitation nowcasting: how atmospheric and satellite sensory data can be used to forecast extreme rainfall hours in advance, providing lead time when every minute matters.

## Flagship Projects

<a href="https://github.com/Shagun-Thakur/AuralQ"><img src="assets/card-auralq.svg" width="100%" alt="AuralQ" /></a>

A deterministic, tool-augmented audio intelligence architecture built to run locally on budget consumer hardware (**RTX 3050, 4 GB**). Local LLM intent parsing (**Ollama `llama3.2:3b`**) is paired with closed-form DSP mathematics (**librosa, SciPy**) and verified by an independent **citation guardrail**.

<details>
<summary><b>Key capabilities &amp; benchmarks</b></summary>
<br/>

| Layer | Approach |
|---|---|
| **Intent parsing** | Local LLM (`llama3.2:3b` via Ollama) with Pydantic schema binding |
| **Computation** | Deterministic closed-form DSP: STFT, spectrograms, MFCCs, Welford online accumulation |
| **Verification** | Independent citation guardrail checks every claim against computed values |
| **Deployment** | Fully local and air-gapped capable; Streamlit interface |

| Evaluation Metric | Measured Result | Benchmark Comparison |
|---|---|---|
| **Citation Grounding Rate** | **99.0%** | vs. 87.8% unaugmented oracle |
| **Numeric Hallucination Rate** | **5.0%** | vs. 20.0% LLM baseline |
| **Abstention Accuracy** | **100.0%** | Safely refuses out-of-scope acoustic claims |
| **Peak VRAM Allocation** | **< 2.4 GB** | Engineered for budget 4 GB VRAM GPUs (RTX 3050) |
| **Average End-to-End Latency** | **< 6.7s** | Single-shot intent parsing + DSP execution |
| **Dataset Profiler Memory** | **< 100 MB** | Welford online accumulation (up to 2,000 files) |

</details>

[Repository](https://github.com/Shagun-Thakur/AuralQ) · [Live Studio Demo](https://auralq-r77uc2bkz7wgu7yifqkduu.streamlit.app/)

<br/>

<a href="https://github.com/Shagun-Thakur/EchoGuard"><img src="assets/card-echoguard.svg" width="100%" alt="EchoGuard" /></a>

A research-oriented pipeline investigating how evidence-based, multi-method feature engineering and deep generative models detect anomalies in industrial acoustic environments, using the **MIMII dataset**.

- Analyzes **temporal, spectral, and cepstral** representations across pumps, fans, valves, and slide rails.
- Investigates deep unsupervised architectures, including **Autoencoders** and **Normalizing Flows**, to detect anomalous machine states without labeled defect data.

[Repository](https://github.com/Shagun-Thakur/EchoGuard)

## Applied Machine Learning & Systems

| Project | What it does | Focus |
|---|---|---|
| [**GlycoScan**](https://github.com/Shagun-Thakur/GlycoScan) · [demo](https://glycoscan-k7jecpfxz98wveubzmfayp.streamlit.app/) | Streamlit dashboard combining clinical reference-range checks with a Random Forest model (Pima Indians Diabetes Database) for risk estimates, feature importance, and parameter flags. | Machine Learning · Health Analytics |
| [**Customer Churn Prediction**](https://github.com/Shagun-Thakur/Customer-churn-prediction) | End-to-end churn platform with model benchmarking (XGBoost, Random Forest), explainability, and an interactive Streamlit interface. | Machine Learning · Explainability |
| [**Smart Home OpenEnv**](https://github.com/Shagun-Thakur/smart-home-openenv) | Custom simulation environment for training RL agents to optimize residential energy use against dynamic electricity tariffs. | Reinforcement Learning |
| [**Multi-Sensor Industrial Monitoring**](https://github.com/Shagun-Thakur/Multi--Sensor-IoT-ML-Industrial-Monitoring-System) | Real-time IoT and ML system for predictive degradation tracking and anomaly detection. | IoT · Anomaly Detection |
| [**AI Voice Assistant**](https://github.com/Shagun-Thakur/AI_Voice_Assistant) | Multilingual voice assistant that processes spoken queries and responds with natural-sounding speech. | Speech Processing · NLP |

## Technical Toolkit

| Area | Tools |
|---|---|
| **Languages** | Python · C++ · SQL|
| **Audio AI & signal processing** | Librosa · SciPy Signal · NumPy · STFT / Spectrograms · MFCCs · Feature Extraction |
| **ML & deep learning** | PyTorch · TensorFlow · Scikit-learn · XGBoost · Random Forest · Autoencoders · Normalizing Flows · Statistical Learning |
| **Grounded AI & local LLMs** | Ollama (`llama3.2:3b`) · Pydantic Schema Binding · Citation Guardrails · Deterministic Tool Augmentation · Air-Gapped Workflows |
| **Deployment & tools** | Streamlit · Docker · Git · GitHub · Hugging Face · Linux |

## Let's Connect

I'm always glad to discuss Machine Learning, Audio AI, signal processing, and verifiable intelligent systems.

[LinkedIn](https://www.linkedin.com/in/shagun-thakur-8509b7281) · [Email](mailto:12shagun2005@gmail.com) · [GitHub](https://github.com/Shagun-Thakur)
