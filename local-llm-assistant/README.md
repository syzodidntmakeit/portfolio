# 🧠 Local LLM Assistant: Running Mistral 7B Locally

Deploying a fully offline personal AI assistant powered by **Mistral 7B** and **Ollama**, secured on Arch Linux. This project focuses on deploying quantized LLMs for private, low-latency inference without relying on cloud APIs.

---

## 🔧 Tech Stack
- **Mistral 7B (Q4_K_M GGUF)**
- **Ollama** for model management
- **LM Studio** (optional GUI)
- **Arch Linux**
- **Docker (optional)**
- **Python, Bash**

---

## 🧪 Features
- Full offline model inference
- CLI and API interface
- Local hosting with `localhost:11434`
- Shell script automation
- Works with `curl`, custom scripts, and frontends

---

## 🧠 What I Learned
- How to deploy LLMs without OpenAI or Google APIs
- Inference optimization using quantization formats
- System resource management for AI workloads
- Privacy-preserving AI architecture

---

## 🛠 Setup Guide
```bash
# Install Ollama
curl https://ollama.com/install.sh | sh

# Run model
ollama run mistral

# Test API
curl http://localhost:11434/api/generate -d '{
  "model": "mistral",
  "prompt": "Explain to me quantum tunneling in Minecraft terms"
}'
