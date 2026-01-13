# Sarcastic AI - The Savage Headline Converter
> This AI is trained to be disrespectful, witty, and sarcastic. Proceed with a sense of humor.

## Overview
**Sarcastic AI** is a fine-tuned Large Language Model (LLM) designed to take boring, neutral news headlines and rewrite them into savage, sarcastic commentary.

It is built on top of Microsoft's **Phi-3 Mini (3.8B)**, fine-tuned using **Unsloth** for efficiency, and deployed as a serverless app using **Streamlit** and **Hugging Face Spaces**.

---

## ✨ Features
- **Savage Mode:** Converts plain text into high-quality sarcasm.
- **Lightweight:** Uses a 4-bit quantized version of Phi-3 for fast inference.
- **Custom System Prompt:** Enforces a specific "witty & disrespectful" persona.
- **Serverless Architecture:** No dedicated GPU required for inference; runs on Hugging Face's free router.
- **Adjustable Parameters:** Control the "Creativity" (Temperature) and length of the sarcasm via the UI.

---

## 📊 Model Evaluation

The model has been rigorously evaluated using both quantitative metrics and qualitative LLM-as-judge assessment.

### Quantitative Metrics
Evaluated on 30 test examples:
- **Average Loss:** 1.8928
- **Perplexity:** 6.64

The low perplexity score indicates that the model generates coherent, natural-sounding sarcastic text with high confidence.

### LLM-as-Judge Evaluation
Using **Gemini 2.5 Flash** as the judge, the model achieved:
- **Final Sarcasm Score:** 4.5 / 5.0

#### Sample Evaluations:

| Headline | Sarcastic Response | Judge Score |
|----------|-------------------|-------------|
| The Human Resources department... | Oh, joy! The Human Resources department has decide... | 4/5 |
| The municipal city council has... | Oh, joy. The city council has decided that the mos... | 5/5 |
| Tech giant reveals their lates... | Oh, how delightful! The tech giant has finally dec... | 4/5 |
| Financial experts suggest that... | Oh, absolutely. Because who needs electricity and ... | 5/5 |

The model demonstrates strong performance in generating contextually appropriate sarcasm with varied sentence structures and witty commentary.

---

## Live Demo
You can try the live application here:

**[Launch Sarcastic AI on Hugging Face](https://hg-goswami-sarcastic-ai-bb50cff.hf.space/?__theme=system&deep_link=M0LWEuaiXlo)**
 
**[See training loss of model](https://api.wandb.ai/links/agentic_error/og6jqbf2)**

**[Download model from here]([hg-goswami/sarcastic-phi3](https://huggingface.co/hg-goswami/sarcastic-phi3))**

*(Note: If the model is "cold," it may take 30-40 seconds to wake up for the first request.)*

---

## 🛠️ Technology Stack
- **Model:** [Phi-3 Mini 3.8B](https://huggingface.co/microsoft/Phi-3-mini-4k-instruct)
- **Fine-Tuning:** [Unsloth](https://github.com/unslothai/unsloth) (LoRA + QLoRA)
- **Training Platform:** Google Colab
- **Model Hosting:** Hugging Face
- **Frontend:** [Streamlit](https://streamlit.io/)
- **Inference:** Hugging Face Serverless Inference API

---
