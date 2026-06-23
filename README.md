<div align="center">

# 🏛️ RoboExhibit

**AI-Powered Interactive Museum Guide**

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org)
[![HuggingFace](https://img.shields.io/badge/🤗-Transformers-yellow.svg)](https://huggingface.co/)
[![RDF](https://img.shields.io/badge/Knowledge-RDF%2FSPARQL-green.svg)](https://www.w3.org/RDF/)
[![Unity](https://img.shields.io/badge/Unity-3D-black.svg)](https://unity.com/)
[![License: GPL-3.0](https://img.shields.io/badge/License-GPL--3.0-blue.svg)](LICENSE)

*AI & Robotics — University of Palermo*

</div>

---

## 📋 Overview

RoboExhibit is an AI-driven interactive museum experience that combines **ontology-based knowledge representation**, **natural language processing**, and **real-time visitor adaptation**. A virtual robot guide navigates a 3D museum in Unity, answers visitor questions using SPARQL queries over an RDF knowledge base, and generates human-like responses through LLMs.

## ✨ Key Features

- 🧠 **Semantic Knowledge Base** — RDF ontology with SPARQL-based information retrieval
- 🗣️ **Natural Language Interaction** — LLM-powered conversational responses (via HuggingFace)
- 🎮 **Immersive 3D Environment** — Unity-based virtual museum with interactive exhibits
- 🔄 **Adaptive Behavior** — Real-time visitor profiling and personalized guided tours

## 🏗️ Architecture

```
┌──────────────┐     ┌───────────────┐     ┌──────────────┐
│  Unity 3D    │────▶│  Backend API  │────▶│  RDF/SPARQL  │
│  (Frontend)  │◀────│  (app.py)     │◀────│  Knowledge   │
└──────────────┘     └───────┬───────┘     └──────────────┘
                             │
                     ┌───────▼───────┐
                     │  HuggingFace  │
                     │  LLM Pipeline │
                     └───────────────┘
```

## 📁 Project Structure

```
├── app.py                              # Backend: API + NLP + SPARQL pipeline
├── Ontologia.rdf                       # Semantic knowledge base
├── Documentazione RoboExhibit.pdf      # Full project report
├── Progetto RoboticaIA2.pptx           # Project presentation
├── Diagramma delle classi.asta         # UML class diagram
└── LICENSE
```

## 🚀 Quick Start

### Prerequisites
- Python 3.10+
- A valid [HuggingFace API token](https://huggingface.co/settings/tokens)

### Running the Backend

```bash
# Set your HuggingFace API key
export HF_API_KEY="your_token_here"

# Install dependencies
pip install flask rdflib transformers torch

# Start the server
python app.py
```

### Unity Frontend

The Unity project is available separately:
📦 [Download from Google Drive](https://drive.google.com/drive/folders/1RwsfyaBKtPtwyXdXrcuHWLGNexv6quj4?usp=sharing)

## 🎬 Demo

▶️ [Watch on YouTube](https://youtu.be/Yx5UH_NVQaA)

## 👥 Authors

- **Antonio Spedito** — [@ashenclock](https://github.com/ashenclock)
- **Alessandro Picone**
- **Lucrezia Mosca**

## 📜 License

This project is licensed under the GPL-3.0 License — see the [LICENSE](LICENSE) file for details.
