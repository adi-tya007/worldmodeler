# 🌍 Autonomous World Modeler

**Simulate alternate futures using generative AI, real-time data retrieval, and interactive scenario control.**

---

##  Project Overview

Autonomous World Modeler is a generative AI system that allows users to explore possible future scenarios by adjusting key global variables such as:

- Climate investment
- Economic growth
- Technology adoption
- Population shifts
- Geopolitical stress

It combines real-time data with structured analysis and large language models (LLMs) to generate human-readable forecasts.

---

##  Features

- Interactive **Gradio** UI for scenario input/output
- Model-backed reasoning using **Mistral-7B Instruct** (GGUF format)
- PDF reporting with graphs and narrative insights
- Counterfactual simulation engine
- Supports offline inference with **ctransformers**

---

##  Setup Instructions
**recommended to run on google colab**

1. Clone this repo and enter the project folder.

```bash
git clone https://github.com/yourusername/world-modeler.git
cd world-modeler
```

2. Install required Python packages:

```bash
pip install gradio ctransformers fpdf sentence-transformers scikit-learn matplotlib
```

3. Download the Mistral-7B Instruct (Q4_K_M) model file:

```bash
wget -O mistral-7b-instruct-v0.1.Q4_K_M.gguf \
https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.1-GGUF/resolve/main/mistral-7b-instruct-v0.1.Q4_K_M.gguf
```

4. Run the notebook .

---

##  Model Information

- **Model**: Mistral-7B Instruct (quantized, `Q4_K_M`)
- **Backend**: `ctransformers` with GGUF support
- **Hardware**: Runs on CPU with 8GB+ RAM (GPU optional for faster inference)

---
##  How It Works

1. You input a base scenario (e.g., “Climate change is reversed by 2050”).
2. Adjust policy sliders like tech adoption, regulation, and investment.
3. The model (Mistral-7B) generates 3 alternate futures.
4. Each future is evaluated across 8 metrics: probability, impact, economy, environment, etc.
5. Results are visualized in a radar chart and compiled into a downloadable PDF report.

##  License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for more information.
