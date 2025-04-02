# VNJPTranslate: A Large-Scale Vietnamese-Japanese Translation System

## 🌟 Table of Contents
1. [Overview](#overview)
2. [Dataset](#dataset)
3. [Report](#report)
4. [Models](#models)

---

## 🌟 Overview <a name="overview"></a>

VNJPTranslate is a system that includes a **Vietnamese-Japanese dataset with 3.3 million sentence pairs**—the largest dataset of its kind. It is designed to be **scalable in both quantity and quality** while utilizing a **lightweight fine-tuned LoRa model** for large-scale translation between Vietnamese and Japanese. The system is optimized for low-cost inference, running efficiently on **small, free GPUs available on Colab and Kaggle**.

---

## 📊 Dataset <a name="dataset"></a>

The VNJPTranslate dataset includes:

- **3.3 million bilingual sentence pairs**, collected from **trusted sources** such as Japanese Wikipedia and Japanese LLM datasets.

- **Download the dataset on Hugging Face**: [VNJPTranslate Corpus on Hugging Face](https://huggingface.co/datasets/haiFrHust/VNJPTranslate)

---

## 📝 Report <a name="report"></a>

For a detailed explanation of our methodology and processes, check out our report on arXiv:

- **Report**: [VNJPTranslate Report](https://arxiv.org/abs/2504.00339)

---

## 🚀 Models <a name="models"></a>

- **Base Model**: Built on the **Qwen 2.5 architecture** and fine-tuned with:
  - **Chain-of-Thought (CoT) prompting**.
  - Two additional datasets: a **Vietnamese version of Alpaca** and a **Japanese question-answer dataset** from Hugging Face.

- Below is our base model. We are actively improving it to achieve even better performance in the near future!  
  + **Model Link**: [Base Model on Hugging Face](https://huggingface.co/haiFrHust/VNJPTranslate_base)

- **Best Model Performance**: Achieved a **BLEU score of 28.3** on the Tatoeba test set, significantly outperforming Opus-MT-Ja-Vi’s **20.3**.

We are continuously improving our models to ensure they remain lightweight and highly efficient.

---
