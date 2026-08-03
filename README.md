# 🧠 MeetMe

> Building a Personal AI Digital Twin using Fine-Tuning, LoRA, and Open-Source LLMs.

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Unsloth](https://img.shields.io/badge/Unsloth-QLoRA-orange)
![Qwen](https://img.shields.io/badge/Qwen-2.5--3B-green)
![License](https://img.shields.io/badge/License-MIT-yellow)

---

## 🚀 Overview

MeetMe is an experimental project that explores whether a relatively small, carefully curated dataset can teach an open-source LLM to respond in a way that reflects a person's communication style, reasoning, and decision-making process.

Instead of building another chatbot, the goal is to build a **Personal AI Digital Twin**.

---

## ✨ Features

- 🧠 Personality-aware responses
- 💬 Fine-tuned on personal conversations
- ⚡ QLoRA fine-tuning with Unsloth
- 🤖 Qwen2.5-3B-Instruct base model
- 📚 ChatML formatted dataset
- 🔒 Fully open-source pipeline
- 🚀 Runs locally after training

---

# 🏗️ Architecture

```text
Raw Journals
      │
      ▼
Dataset Preparation
      │
      ▼
ChatML Dataset
      │
      ▼
QLoRA Fine-Tuning
      │
      ▼
MeetMe V1
      │
      ▼
Chat Interface
```

---

# 📊 Training Details

| Component | Value |
|------------|-------|
| Base Model | Qwen2.5-3B-Instruct |
| Fine-Tuning | SFT |
| Method | QLoRA |
| Framework | Unsloth |
| Dataset | 171 Samples |
| Format | ChatML |
| Hardware | Google Colab T4 |

---

# 📂 Dataset

The dataset was manually curated from:

- Personal journals
- Notes
- Conversations
- Reflections

Every sample follows ChatML.

Example

```json
{
  "messages":[
    {
      "role":"user",
      "content":"How do you learn new technologies?"
    },
    {
      "role":"assistant",
      "content":"I like breaking complex topics into systems..."
    }
  ]
}
```

---

# 🛠 Tech Stack

- Python
- Transformers
- PEFT
- TRL
- Unsloth
- BitsAndBytes
- Hugging Face
- Google Colab

---

# 📈 Current Results

Current Version:

MeetMe V1

Training Samples:

171

Evaluation:

- Personality
- Learning Style
- Decision Making
- Communication
- Reflection

The first version successfully demonstrates early personality transfer while keeping the base model's reasoning capabilities.

---

# 🗺 Roadmap

- [x] Dataset Collection
- [x] ChatML Conversion
- [x] QLoRA Fine-tuning
- [x] First Evaluation
- [ ] 1000+ Samples
- [ ] RAG Integration
- [ ] Long-Term Memory
- [ ] Voice Interface
- [ ] Streamlit UI
- [ ] Local Deployment
- [ ] Continuous Learning

---

# 💡 What I Learned

The biggest lesson from this project wasn't about choosing the best model.

It was understanding that **the quality of an AI model starts with the quality of its data**.

Preparing the dataset required significantly more effort than the actual fine-tuning process, reinforcing the importance of data curation in modern AI systems.

---

# ⚠️ Limitations

- Small training dataset (171 samples)
- No persistent memory
- No Retrieval-Augmented Generation (RAG)
- Responses may still reflect the base model outside trained topics

---

# 🤝 Contributing

This project is currently a personal research experiment.

Suggestions, discussions, and feedback are always welcome.

---

# 📬 Contact

**Sanskar**

LinkedIn: https://linkedin.com/in/YOUR_USERNAME

Hugging Face: https://huggingface.co/YOUR_USERNAME

GitHub: https://github.com/YOUR_USERNAME

---

⭐ If you found this project interesting, consider giving it a star!