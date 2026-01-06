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

## Live Demo

You can try the live application here:

 **[Launch Sarcastic AI on Hugging Face](https://hg-goswami-sarcastic-ai-bb50cff.hf.space/?__theme=system&deep_link=M0LWEuaiXlo)**
 
 **[See training loss of model](https://api.wandb.ai/links/agentic_error/og6jqbf2)**

*(Note: If the model is "cold," it may take 30-40 seconds to wake up for the first request.)*

---

## 🛠️ Technology StackLooks like you stumbled on an empty page.
If this is the right URL, you might need to ask the page owner to change the privacy permissions or invite you to

- **Model:** [Phi-3 Mini 3.8B](https://huggingface.co/microsoft/Phi-3-mini-4k-instruct)
- **Fine-Tuning:** [Unsloth](https://github.com/unslothai/unsloth) (LoRA + QLoRA)
- **Frontend:** [Streamlit](https://streamlit.io/)
- **Inference:** Hugging Face Serverless Inference API

---
