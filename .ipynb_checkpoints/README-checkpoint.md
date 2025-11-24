# AI-ML-Assignment-4 — Generative LLM Experiment  
**Author:** Kyle Kitching  
**Model Used:** `openai-community/gpt2`  
**Task Type:** Text Generation

---

## 📌 Overview
The goal of this project is to gain hands-on experience using a pre-trained Large Language Model (LLM) via the Hugging Face Transformers library. I selected GPT-2 and implemented a text generation task. The experiment focuses on how modifying **temperature** affects creativity, coherence, and style in generated text.

---

## 📦 Project Structure
├── llm_text_generation.ipynb
└── README.md

## 🧪 Experiment Setup

### Base Prompt
"You are an aspiring software engineer learning about large language models. 
Write a short, imaginative story about how training an AI model helped you 
start a new chapter in your life."

### Fixed Parameters
- max_new_tokens = 120
- top_p = 0.9
- do_sample = True
- Model: GPT-2 Small (openai-community/gpt2)

The only parameter varied was **temperature**.

## 🔬 Temperature Experiment Results

### Result Summary Table

| Temperature | Output Snippet | Observation |
|------------|----------------|-------------|
| **0.2** | You are an aspiring software engineer learning about large language models. Write a short, imaginative story about how training an AI model helped you start a new chapter in your life.| Predictable, coherent, low creativity |
| **0.7** | You are an aspiring software engineer learning about large language models. Write a short, imaginative story about how training an AI model helped you start a new chapter in your life. | Balanced, descriptive, natural |
| **1.0** | You are an aspiring software engineer learning about large language models. Write a short, imaginative story about how training an AI model helped you start a new chapter in your life. You will also learn about the role of social capital in AI technology. | Creative, surprising, sometimes incoherent |

## 📝 Analysis

### Temperature 0.2
- Very conservative
- Predictable and repetitive
- Highly coherent, low creativity

### Temperature 0.7
- Best balance
- Good detail and flow
- Natural storytelling

### Temperature 1.0
- Most creative
- Adds random or surprising elements
- Sometimes loses coherence

## 🎯 Conclusion
This project demonstrated how temperature strongly influences generative model behavior. Low temperatures produced predictable but uncreative output, while medium temperatures gave the best balance of coherence and imagination. At high temperatures, the model became more creative but less consistent. Overall, temperature 0.7 generated the best results for a story-writing task.

## 🛠️ Technologies Used
- Hugging Face Transformers
- PyTorch
- Google Colab / Jupyter Notebook
- GPT-2 (Causal Language Model)

## 📚 References
- https://huggingface.co/docs/transformers
- https://huggingface.co/openai-community/gpt2
- https://huggingface.co/blog/how-to-generate
- 
## ▶️ Video Demonstration
Link: https://youtu.be/7oxneKFqnYU



