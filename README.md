# MemInsight: Autonomous Memory Augmentation for LLM Agents

MemInsight is a structured memory augmentation framework designed to enhance the long-term reasoning and adaptability of large language model (LLM) agents. It introduces autonomous memory annotation and retrieval methods that help agents organize and access relevant historical context during inference.

---

## 🔍 Overview

As LLM agents scale, managing accumulated memory across diverse interactions becomes a major challenge. MemInsight addresses this by:

- **Autonomously generating structured memory augmentations**
- **Prioritizing semantically rich attributes for retrieval**
- **Improving memory relevance with attribute-based and embedding-based methods**
- **Boosting response quality in recommendation, QA, and summarization tasks**

---

## 🧩 Key Features

- **Attribute Mining**: Extracts entity- and conversation-centric attributes from dialogues
- **Memory Annotation**: Supports both turn-level and session-level augmentation
- **Retrieval Methods**:
  - Attribute-Based Filtering
  - Embedding-Based Similarity (FAISS)
- **Task Support**:
  - Conversational Recommendation
  - Question Answering
  - Event Summarization

---

## 📈 Benchmark Results

MemInsight outperforms traditional memory retrieval methods:

| Task                    | Metric           | Improvement |
|-------------------------|------------------|-------------|
| QA (LoCoMo)             | Recall@5         | +34% over DPR |
| Conversational Reco.    | Persuasiveness   | +14%         |
| Event Summarization     | G-Eval (Relevance) | Comparable to baseline with less memory |

---

## 📂 Datasets Used

- [LLM-REDIAL](https://huggingface.co/datasets/LLM-REDIAL): Movie recommendation dataset
- [LoCoMo](https://arxiv.org/abs/2402.17753): Multi-turn long-context QA and summarization

---

## 🛠️ Setup

```bash
git clone https://github.com/<your-org>/meminsight.git
cd meminsight
pip install -r requirements.txt
