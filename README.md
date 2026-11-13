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

I'm a Computer Science undergraduate who builds machine learning systems for **real-world physical signals**: sound, vibration and sensor time series. I care about two things: making results **verifiable** (grounded outputs, fixed seeds, statistical tests) and reporting them **honestly**, including the cases where a simple baseline wins.

**What I work on**
- **Audio AI:** unsupervised anomaly detection, emergency-sound detection, speech pipelines (STT/TTS)
- **Grounded AI:** pairing local LLMs with deterministic DSP and citation guardrails to cut numeric hallucinations
- **Evaluation:** multi-seed protocols, paired significance tests, reproducibility checks
- **Efficient AI:** systems that run locally on consumer hardware (under 4 GB VRAM)

## Current Research

How do signal representations, learning methods, and deterministic guardrails interact to make ML systems reliable in real sensory environments?

- **Audio AI & acoustic grounding:** eliminating acoustic hallucinations by pairing local LLMs with closed-form DSP algorithms behind strict citation guardrails.
- **Unsupervised anomaly detection:** representation learning, generative modeling, and multi-method feature extraction on complex industrial soundscapes.
- **Resource-constrained AI:** high-efficiency architectures that run locally on consumer-grade hardware (sub-4 GB VRAM).

### Field research: Project Tarini (precipitation nowcasting)

<img src="assets/card-tarini.svg" width="100%" alt="Project Tarini" />

In flood-vulnerable regions such as the Brahmaputra basin in Assam, extreme monsoon downpours and sudden cloudbursts can trigger catastrophic flash floods within hours, putting communities, agriculture, and infrastructure at severe risk.

Traditional numerical weather forecasting often lacks the rapid, localized granularity that emergency response requires. **Project Tarini** is an ongoing research initiative investigating spatio-temporal precipitation nowcasting: how atmospheric and satellite sensory data can be used to forecast extreme rainfall hours in advance, providing lead time when every minute matters.

## Flagship Projects

<a href="https://github.com/Shagun-Thakur/AuralQ"><img src="assets/card-auralq.svg" width="100%" alt="AuralQ" /></a>

A local, tool-augmented system for asking natural-language questions about audio, built to run locally on budget consumer hardware (**RTX 3050, 4 GB**). A local LLM (Ollama, `llama3.2:3b`) only parses intent. All numbers come from closed-form DSP (librosa, SciPy), and an independent citation guardrail checks every number in the answer against the computed values.

<details>
<summary><b>Key capabilities &amp; benchmarks</b></summary>
<br/>

| Metric (20-case benchmark) | LLM only (B2) | Fixed pipeline (B3) | **AuralQ (B4)** |
|---|:---:|:---:|:---:|
| Citation grounding rate | 90.0% | 94.4% | **99.0%** |
| Numeric hallucination rate | 10.0% | 10.0% | **5.0%** |
| Abstention accuracy | 90.0% | 90.0% | **100.0%** |

Runs under 2.4 GB VRAM (RTX 3050), about 6.7 s end to end, with 74 passing tests. *Small benchmark (20 cases): treat the gaps as indicative, not statistically established.*

</details>

[Repository](https://github.com/Shagun-Thakur/AuralQ) · [Live Studio Demo](https://auralq-r77uc2bkz7wgu7yifqkduu.streamlit.app/)

<br/>

<a href="https://github.com/Shagun-Thakur/EchoGuard"><img src="assets/card-echoguard.svg" width="100%" alt="EchoGuard" /></a>

A research-oriented pipeline on the **MIMII** dataset (pumps, fans, valves, slide rails). It compares temporal, spectral and cepstral acoustic representations and deep unsupervised models (**Autoencoders** and **Normalizing Flows**) to detect faulty machine states without labelled defect data.

[Repository](https://github.com/Shagun-Thakur/EchoGuard)

<br/>

<a href="https://github.com/Shagun-Thakur/smart-home-openenv"><img src="assets/card-smarthome.svg" width="100%" alt="Smart Home OpenEnv" /></a>

A Gymnasium environment for HVAC and battery control under time-of-use pricing, with thermal inertia and Markov occupancy. Evaluated with **10 training seeds**, **50 disjoint evaluation seeds** and **Wilcoxon signed-rank tests**. Retraining reproduces bit-identical weights, and a 38-test suite guards physics, determinism and checkpoint integrity.

The honest finding: PPO beats the rule-based heuristics but is statistically indistinguishable from a constant 24°C baseline (p = 0.789); DQN trails PPO at both training budgets. The README lists seven threats to validity. Deployed with FastAPI and Docker on Hugging Face Spaces.

[Repository](https://github.com/Shagun-Thakur/smart-home-openenv)

## Collaboration

<a href="https://github.com/Anjalisahni24/ResQ_Audio_ANNapp"><img src="assets/card-resq.svg" width="100%" alt="ResQ" /></a>

Built the core machine-learning engine for emergency sound detection—handling acoustic data preparation, feature extraction, and neural network model training for integration into the companion Android app developed by [@Anjalisahni24](https://github.com/Anjalisahni24).

[Repository](https://github.com/Anjalisahni24/ResQ_Audio_ANNapp)

<br/>

<a href="https://github.com/AnonAjay/Jaanch"><img src="assets/card-jaanch.svg" width="100%" alt="Jaanch" /></a>

Contributed to the voice-assisted form verification Chrome extension by resolving cross-origin iframe microphone permission constraints and fixing stream-handling bugs across the speech-to-text (STT) and text-to-speech (TTS) API pipeline.

[Repository](https://github.com/AnonAjay/Jaanch)

## More Projects

| Project | What it does | Focus |
|---|---|---|
| [**GlycoScan**](https://github.com/Shagun-Thakur/GlycoScan) · [demo](https://glycoscan-k7jecpfxz98wveubzmfayp.streamlit.app/) | Streamlit dashboard combining clinical reference-range checks with a Random Forest risk model (Pima Indians Diabetes dataset) for risk estimates, feature importance, and parameter flags. *Educational demo, not medical advice.* | Tabular ML · Health Analytics |
| [**Customer Churn Prediction**](https://github.com/Shagun-Thakur/Customer-churn-prediction) | End-to-end churn platform with model benchmarking (XGBoost, Random Forest), explainability, and an interactive Streamlit interface. | ML · Explainability |
| [**Multi-Sensor Industrial Monitoring**](https://github.com/Shagun-Thakur/Multi--Sensor-IoT-ML-Industrial-Monitoring-System) | Real-time IoT and ML system for predictive degradation tracking, anomaly detection, and automated failure handling. | IoT · Anomaly Detection |
| [**AI Voice Assistant**](https://github.com/Shagun-Thakur/AI_Voice_Assistant) | Multilingual voice assistant that processes spoken queries and responds with natural-sounding speech across multiple languages. | Speech Processing · NLP |

## Technical Toolkit

| Area | Tools |
|---|---|
| **Languages** | Python · C++ · SQL |
| **Audio AI & signal processing** | Librosa · SciPy Signal · NumPy · STFT / Spectrograms · MFCCs · Feature Extraction |
| **ML & deep learning** | PyTorch · TensorFlow · Scikit-learn · XGBoost · Random Forest · Autoencoders · Normalizing Flows · Statistical Learning |
| **Reinforcement learning** | Gymnasium · Stable-Baselines3 (PPO, DQN) · Custom Environment Design |
| **Grounded AI & local LLMs** | Ollama (`llama3.2:3b`) · Pydantic Schema Binding · Citation Guardrails · Deterministic Tool Augmentation · Air-Gapped Workflows |
| **Speech & integration** | STT/TTS APIs · FastAPI · Chrome Extension Development & Debugging |
| **Deployment & workflow** | Streamlit · Docker · Hugging Face Spaces · Git · Linux · pytest |

## Let's Connect

I'm always glad to discuss Machine Learning, Audio AI, signal processing, and verifiable intelligent systems.

[LinkedIn](https://www.linkedin.com/in/shagun-thakur-8509b7281) · [Email](mailto:thakurshagun412@gmail.com) · [GitHub](https://github.com/Shagun-Thakur)
