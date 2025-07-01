# 🧠 Contextual Entity Resolution Project

**Author:** Zachary L. Johnson-Scott  
**Disclaimer:** The core ideas and methodology are my own. AI tools were used to assist with content structuring and refinement for clarity and speed.

---

## 📌 Problem Statement

Traditional entity resolution relies on static identifiers (e.g., names, emails, IDs), which fails in disconnected, unstructured, or anonymized data environments. This limitation is especially critical in domains such as influence analysis or intelligence, where aliases and obfuscation are common.

---

## 💡 Solution Overview

This project proposes a **Generative AI-powered pipeline** for resolving entities based on **contextual and behavioral similarity**, not just names. By leveraging tools like **LangChain** and **Retrieval-Augmented Generation (RAG)**, we can infer connections between seemingly unrelated entities through shared patterns of life, semantic context, and domain-specific indicators.

### Example

Instead of matching `"Taylor Swift"` and `"TayTay13"` by name, the system examines:
- Posting behavior  
- Content themes (e.g., song lyrics, poetry)  
- Co-occurrence with known entities  
- Temporal engagement patterns  

This method enhances resilience in environments with:
- Pseudonyms  
- Anonymized reporting  
- Alias usage  

---

## 🛠️ Technical Approach

### 🔧 Components

- **Custom Embeddings & Vector Search**  
  Tailored embeddings for behavioral and thematic domains.

- **RAG Pipeline with LangChain**  
  Retrieves contextual evidence from stored documents for reasoning.

- **Entity Similarity Scoring**  
  Compares behavior, semantic content, and (optional) metadata to resolve alignment.

- **Optional Fine-Tuning**  
  Uses labeled examples or reinforcement learning to improve accuracy.
---

## 🧪 Experiment: Behavior-Based Entity Resolution

### 🎯 Objective

Test contextual entity resolution using synthetic yet realistic activity patterns, aliases, and RAG pipelines.

### 🏗️ Setup

- **Synthetic Data Generation:** Used ChatGPT & Gemini to simulate real-world personas and behavior.  
- **Vector Database:** Stored embeddings in **Chroma** using pre-trained models (HuggingFace, OpenAI, Ollama LLaMA3).  
- **Metadata Example:**

```json
{
  "True_Name": "Taylor Swift",
  "Aliases": ["TayTay13", "T.S.", "The Tortured Poet"],
  "Activity": "Went to Oakdale Park on the 4th of July and sang 'Mad Love'."
}
```

- **Obfuscated Query Example:**

```
“Which artist appeared in a Twin Cities park on Independence Day and sang about obsessive love?”
```

### ✅ Results

- **Successful entity resolution** despite:
  - Alias masking  
  - Distractor entities  
  - Absence of direct identifiers  

---

## 🚀 Roadmap

### 🧩 Phase 1: Single Entity Resolution

- ✅ Entity resolution using behavioral and contextual similarity  
- Demonstrated retrieval accuracy using RAG + embeddings

### 🔄 Phase 2: Alias Binning & Canonical Identity Creation

- 🚧 Clustering logic to unify aliases into one canonical entity  
- Uses similarity scores, timeline overlap, and metadata fusion

### 🌐 Phase 3: Network Graph & Relational Linking

- 🔜 Construct behavioral network graphs of related entities  
- Connects nodes via shared activity, influence pathways, or co-occurrence

---

## 🧠 Key Applications

- Influence Operations & PsyOps  
- Human Terrain Mapping  
- Population Behavior Analysis  
- Marketing & Consumer Behavior Intelligence  
- Anonymized Social Media Profiling  

---

## 🧾 Conclusion

This experiment validates that **Generative AI + Vector Similarity** can perform soft entity resolution with high potential in real-world applications. While built on synthetic data, this approach offers:

- Robust handling of pseudonyms and obfuscation  
- Scalable architecture for future knowledge graph and RL integration  
- Practical use in intelligence, marketing, and behavioral science  

---

## 🔗 Tools & Frameworks

- [LangChain](https://www.langchain.com/)  
- [Chroma](https://www.trychroma.com/)  
- [HuggingFace Transformers](https://huggingface.co/)  
- [OpenAI API](https://platform.openai.com/)  
- [Ollama LLaMA3](https://ollama.com/)  

---

## 📬 Contact

**Zachary L. Johnson-Scott**  
Data & AI Strategist | Influence Technologist  
📍 Lakeville, MN  
📧 zachary.johnsonscott@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/zachary-johnson-scott-94a58029a)

---

