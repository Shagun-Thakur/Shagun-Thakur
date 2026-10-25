<!--
  PROFILE README: Shagun Thakur
  Theme: electric yellow #FFCB05 · ink #0D1117 · accent red #E63946
-->

<div align="center">
  <img src="assets/header.svg" width="100%" alt="Shagun Thakur: Machine Learning, Audio AI, Intelligent Systems" />
  <br/><br/>
  <a href="https://www.linkedin.com/in/shagun-thakur-8509b7281"><img src="https://img.shields.io/badge/LinkedIn-0D1117?style=for-the-badge&logoColor=FFCB05&logo=linkedin" alt="LinkedIn" /></a>
  <a href="mailto:12shagun2005@gmail.com"><img src="https://img.shields.io/badge/Email-0D1117?style=for-the-badge&logoColor=FFCB05&logo=gmail" alt="Email" /></a>
  <a href="https://auralq-r77uc2bkz7wgu7yifqkduu.streamlit.app/"><img src="https://img.shields.io/badge/%E2%9A%A1%20AuralQ%20Live%20Demo-FFCB05?style=for-the-badge&logoColor=0D1117&labelColor=FFCB05" alt="⚡ AuralQ Live Demo" /></a>
  <a href="https://glycoscan-k7jecpfxz98wveubzmfayp.streamlit.app/"><img src="https://img.shields.io/badge/%E2%9A%A1%20GlycoScan%20Live%20Demo-FFCB05?style=for-the-badge&logoColor=0D1117&labelColor=FFCB05" alt="⚡ GlycoScan Live Demo" /></a>
</div>

<br/>

<img src="assets/sec-about.svg" width="100%" alt="About" />

<table>
  <tr>
    <td width="200" align="center" valign="top">
      <img src="https://github.com/Shagun-Thakur.png?size=300" width="180" alt="Profile avatar" />
    </td>
    <td valign="top">
      <p>I'm a <b>Computer Science undergraduate</b> interested in how machines learn from <b>real-world physical signals</b>: acoustic waves, vibrations, and sensory time series.</p>
      <p>My work spans <b>Machine Learning, Deep Learning, Audio Signal Processing, and Deterministic AI Grounding</b>. I focus on pairing closed-form signal mathematics with modern learning architectures to build <b>verifiable, hallucination-resistant systems</b> that run efficiently on accessible hardware.</p>
    </td>
  </tr>
</table>

<br/>

<img src="assets/sec-research.svg" width="100%" alt="Current Research & Focus" />

How do signal representations, learning methods, and deterministic guardrails interact to make ML systems reliable in real sensory environments?

<table>
  <tr>
    <td><img src="assets/focus-audio.svg" width="100%" alt="Audio AI and Acoustic Grounding" /></td>
    <td><img src="assets/focus-anomaly.svg" width="100%" alt="Unsupervised Anomaly Detection" /></td>
    <td><img src="assets/focus-edge.svg" width="100%" alt="Resource-Constrained AI" /></td>
  </tr>
</table>

<img src="assets/card-tarini.svg" width="100%" alt="Project Tarini: precipitation nowcasting" />

> In flood-vulnerable regions such as the Brahmaputra basin in Assam, extreme monsoon downpours and sudden cloudbursts can trigger catastrophic flash floods within hours, putting communities, agriculture, and infrastructure at severe risk.
>
> Traditional numerical weather forecasting often lacks the rapid, localized granularity that emergency response requires. **Project Tarini** is an ongoing research initiative investigating spatio-temporal precipitation nowcasting: how atmospheric and satellite sensory data can be used to forecast extreme rainfall hours in advance, providing lead time when every minute matters.

<br/>

<img src="assets/sec-flagship.svg" width="100%" alt="Flagship Projects" />

<a href="https://github.com/Shagun-Thakur/AuralQ"><img src="assets/card-auralq.svg" width="100%" alt="AuralQ" /></a>

A deterministic, tool-augmented audio intelligence architecture engineered to run locally on budget consumer hardware (**RTX 3050, 4 GB**). Local LLM intent parsing (**Ollama `llama3.2:3b`**) is paired with closed-form DSP mathematics (**librosa, SciPy**) and verified by an independent **citation guardrail**.

<details>
<summary><b>⚡ Inspect key capabilities &amp; benchmarks</b></summary>
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
| **Peak VRAM Allocation** | **< 2.4 GB** | Engineered for budget 4 GB VRAM GPUs |
| **Average End-to-End Latency** | **< 6.7s** | Single-shot intent parsing + DSP execution |
| **Dataset Profiler Memory** | **< 100 MB** | Welford online accumulation (up to 2,000 files) |

</details>

<a href="https://github.com/Shagun-Thakur/AuralQ"><img src="https://img.shields.io/badge/Repository%20%E2%86%92-FFCB05?style=flat-square&labelColor=FFCB05&color=FFCB05" alt="Repository →" /></a> <a href="https://auralq-r77uc2bkz7wgu7yifqkduu.streamlit.app/"><img src="https://img.shields.io/badge/Live%20Studio%20Demo%20%E2%86%92-FFCB05?style=flat-square&labelColor=FFCB05&color=FFCB05" alt="Live Studio Demo →" /></a>

<br/>

<a href="https://github.com/Shagun-Thakur/EchoGuard"><img src="assets/card-echoguard.svg" width="100%" alt="EchoGuard" /></a>

A research-oriented pipeline investigating how evidence-based, multi-method feature engineering and deep generative models detect anomalies in industrial acoustic environments, using the **MIMII dataset**.

- Analyzes **temporal, spectral, and cepstral** representations across pumps, fans, valves, and slide rails.
- Investigates deep unsupervised architectures, including **Autoencoders** and **Normalizing Flows**, to detect anomalous machine states without labeled defect data.

<a href="https://github.com/Shagun-Thakur/EchoGuard"><img src="https://img.shields.io/badge/Repository%20%E2%86%92-FFCB05?style=flat-square&labelColor=FFCB05&color=FFCB05" alt="Repository →" /></a>

<br/>

<img src="assets/sec-applied.svg" width="100%" alt="Applied ML & Systems" />

<table>
  <tr>
    <td valign="top" width="50%">
      <a href="https://github.com/Shagun-Thakur/GlycoScan"><img src="assets/card-glycoscan.svg" width="100%" alt="GlycoScan" /></a>
      <sub>Streamlit app combining clinical reference-range evaluation with a Random Forest model trained on the Pima Indians Diabetes Database, providing risk estimates, feature-importance insights, and parameter flags.</sub><br/>
      <a href="https://github.com/Shagun-Thakur/GlycoScan"><img src="https://img.shields.io/badge/Repository%20%E2%86%92-FFCB05?style=flat-square&labelColor=FFCB05&color=FFCB05" alt="Repository →" /></a> <a href="https://glycoscan-k7jecpfxz98wveubzmfayp.streamlit.app/"><img src="https://img.shields.io/badge/Live%20Demo%20%E2%86%92-FFCB05?style=flat-square&labelColor=FFCB05&color=FFCB05" alt="Live Demo →" /></a>
    </td>
    <td valign="top" width="50%">
      <a href="https://github.com/Shagun-Thakur/Customer-churn-prediction"><img src="assets/card-churn.svg" width="100%" alt="Customer Churn Prediction" /></a>
      <sub>Production-oriented churn prediction platform with end-to-end ML pipelines, model benchmarking (XGBoost, Random Forest), feature explainability, and an interactive Streamlit interface.</sub><br/>
      <a href="https://github.com/Shagun-Thakur/Customer-churn-prediction"><img src="https://img.shields.io/badge/Repository%20%E2%86%92-FFCB05?style=flat-square&labelColor=FFCB05&color=FFCB05" alt="Repository →" /></a>
    </td>
  </tr>
  <tr>
    <td valign="top">
      <a href="https://github.com/Shagun-Thakur/smart-home-openenv"><img src="assets/card-smarthome.svg" width="100%" alt="Smart Home OpenEnv" /></a>
      <sub>Custom simulation environment for training reinforcement learning agents to optimize residential energy management, balancing occupant comfort against dynamic electricity tariffs.</sub><br/>
      <a href="https://github.com/Shagun-Thakur/smart-home-openenv"><img src="https://img.shields.io/badge/Repository%20%E2%86%92-FFCB05?style=flat-square&labelColor=FFCB05&color=FFCB05" alt="Repository →" /></a>
    </td>
    <td valign="top">
      <a href="https://github.com/Shagun-Thakur/Multi--Sensor-IoT-ML-Industrial-Monitoring-System"><img src="assets/card-sensors.svg" width="100%" alt="Multi-Sensor Industrial Monitoring" /></a>
      <sub>Real-time multi-sensor monitoring system using IoT and machine learning for predictive degradation tracking and anomaly detection.</sub><br/>
      <a href="https://github.com/Shagun-Thakur/Multi--Sensor-IoT-ML-Industrial-Monitoring-System"><img src="https://img.shields.io/badge/Repository%20%E2%86%92-FFCB05?style=flat-square&labelColor=FFCB05&color=FFCB05" alt="Repository →" /></a>
    </td>
  </tr>
  <tr>
    <td valign="top">
      <a href="https://github.com/Shagun-Thakur/AI_Voice_Assistant"><img src="assets/card-voice.svg" width="100%" alt="AI Voice Assistant" /></a>
      <sub>Voice-based assistant that processes spoken natural-language queries and responds with natural-sounding speech across multiple languages.</sub><br/>
      <a href="https://github.com/Shagun-Thakur/AI_Voice_Assistant"><img src="https://img.shields.io/badge/Repository%20%E2%86%92-FFCB05?style=flat-square&labelColor=FFCB05&color=FFCB05" alt="Repository →" /></a>
    </td>
    <td></td>
  </tr>
</table>

<br/>

<img src="assets/sec-toolkit.svg" width="100%" alt="Technical Toolkit" />

**Languages**<br/>
<img src="https://img.shields.io/badge/Python-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05&logo=python" alt="Python" /> <img src="https://img.shields.io/badge/C%2B%2B-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05&logo=cplusplus" alt="C++" /> <img src="https://img.shields.io/badge/SQL-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05" alt="SQL" /> <img src="https://img.shields.io/badge/Bash-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05&logo=gnubash" alt="Bash" />

**Audio AI & Signal Processing**<br/>
<img src="https://img.shields.io/badge/Librosa-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05" alt="Librosa" /> <img src="https://img.shields.io/badge/SciPy%20Signal-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05&logo=scipy" alt="SciPy Signal" /> <img src="https://img.shields.io/badge/NumPy-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05&logo=numpy" alt="NumPy" /> <img src="https://img.shields.io/badge/STFT%20%2F%20Spectrograms-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05" alt="STFT / Spectrograms" /> <img src="https://img.shields.io/badge/MFCCs-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05" alt="MFCCs" /> <img src="https://img.shields.io/badge/Welford%20Online%20Accumulation-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05" alt="Welford Online Accumulation" /> <img src="https://img.shields.io/badge/Feature%20Extraction-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05" alt="Feature Extraction" />

**Machine Learning & Deep Learning**<br/>
<img src="https://img.shields.io/badge/PyTorch-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05&logo=pytorch" alt="PyTorch" /> <img src="https://img.shields.io/badge/TensorFlow-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05&logo=tensorflow" alt="TensorFlow" /> <img src="https://img.shields.io/badge/Scikit--learn-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05&logo=scikitlearn" alt="Scikit-learn" /> <img src="https://img.shields.io/badge/XGBoost-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05" alt="XGBoost" /> <img src="https://img.shields.io/badge/Random%20Forest-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05" alt="Random Forest" /> <img src="https://img.shields.io/badge/Autoencoders-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05" alt="Autoencoders" /> <img src="https://img.shields.io/badge/Normalizing%20Flows-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05" alt="Normalizing Flows" /> <img src="https://img.shields.io/badge/Statistical%20Learning-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05" alt="Statistical Learning" />

**Grounded AI & Local LLMs**<br/>
<img src="https://img.shields.io/badge/Ollama%20%28llama3.2%3A3b%29-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05&logo=ollama" alt="Ollama (llama3.2:3b)" /> <img src="https://img.shields.io/badge/Pydantic%20Schema%20Binding-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05&logo=pydantic" alt="Pydantic Schema Binding" /> <img src="https://img.shields.io/badge/Citation%20Guardrails-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05" alt="Citation Guardrails" /> <img src="https://img.shields.io/badge/Deterministic%20Tool%20Augmentation-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05" alt="Deterministic Tool Augmentation" /> <img src="https://img.shields.io/badge/Air--Gapped%20Workflows-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05" alt="Air-Gapped Workflows" />

**Deployment & Tools**<br/>
<img src="https://img.shields.io/badge/Streamlit-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05" alt="Streamlit" /> <img src="https://img.shields.io/badge/Docker-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05&logo=docker" alt="Docker" /> <img src="https://img.shields.io/badge/Git-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05&logo=git" alt="Git" /> <img src="https://img.shields.io/badge/GitHub-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05&logo=github" alt="GitHub" /> <img src="https://img.shields.io/badge/Hugging%20Face-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05&logo=huggingface" alt="Hugging Face" /> <img src="https://img.shields.io/badge/Linux-0D1117?style=flat-square&labelColor=0D1117&logoColor=FFCB05&logo=linux" alt="Linux" />

<br/>

<img src="assets/sec-connect.svg" width="100%" alt="Let's Connect" />

I'm always glad to discuss Machine Learning, Audio AI, signal processing, and verifiable intelligent systems.

<div align="center">
  <a href="https://www.linkedin.com/in/shagun-thakur-8509b7281"><img src="https://img.shields.io/badge/LinkedIn-0D1117?style=for-the-badge&logoColor=FFCB05&logo=linkedin" alt="LinkedIn" /></a>
  <a href="mailto:12shagun2005@gmail.com"><img src="https://img.shields.io/badge/Email-0D1117?style=for-the-badge&logoColor=FFCB05&logo=gmail" alt="Email" /></a>
  <a href="https://github.com/Shagun-Thakur"><img src="https://img.shields.io/badge/GitHub-FFCB05?style=for-the-badge&logoColor=0D1117&labelColor=FFCB05&logo=github" alt="GitHub" /></a>
</div>

<br/>

<img src="assets/footer.svg" width="100%" alt="Thanks for visiting" />
