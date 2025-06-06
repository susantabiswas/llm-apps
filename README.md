# LLM Applications

A collection of applications and examples leveraging Large Language Models (LLMs) with various frameworks and tools.

## 📋 Table of Contents

- [LLM Applications](#llm-applications)
  - [📋 Table of Contents](#-table-of-contents)
  - [🔍 Overview](#-overview)
  - [🚀 Setup](#-setup)
    - [Prerequisites](#prerequisites)
    - [Installation](#installation)
  - [💻 Applications and Use Cases](#-applications-and-use-cases)
    - [LLM Debater](#llm-debater)
    - [Tool Usage and Function Calling](#tool-usage-and-function-calling)
    - [Voice Responses and Audio Integration](#voice-responses-and-audio-integration)
    - [Agent Systems](#agent-systems)
    - [Prompt Engineering Techniques](#prompt-engineering-techniques)
    - [Retrieval-Augmented Generation (RAG)](#retrieval-augmented-generation-rag)
  - [📚 Notebook Examples](#-notebook-examples)
  - [📦 Dependencies](#-dependencies)

## 🔍 Overview

This repository contains various applications and examples that demonstrate the capabilities of Large Language Models (LLMs) using frameworks like LangChain, OpenAI, Hugging Face Transformers, and more. The projects explore different ways to leverage LLMs for practical applications, showcasing both the technical implementation and real-world use cases.

## 🚀 Setup

### Prerequisites

- Python 3.11 or higher
- CUDA-capable GPU (for optimal performance with PyTorch)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/llm-apps.git
   cd llm-apps
   ```

2. Create a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   # On Windows
   venv\Scripts\activate
   # On macOS/Linux
   source venv/bin/activate
   ```

3. Install dependencies using UV:
   ```bash
   pip install uv

   uv add requirements.txt
   # or
   uv pip install -e .
   ```

   Or using pip:
   ```bash
   pip install -e .
   ```

4. Set up environment variables:
   Create a `.env` file in the root directory with your API keys. 
   You can use the `.env-example` as the template and fill the API keys and tokens accordingly in it and rename it to `.env`:


5. Start Jupyter Notebook or JupyterLab to explore the notebooks:
   ```bash
   jupyter notebook
   # Or
   uv run --with jupyter jupyter lab
   ```

## 💻 Applications and Use Cases

This repository includes various applications and examples that demonstrate different capabilities of LLMs:

### LLM Debater

The repository includes an implementation of an LLM-powered debate system that can argue different perspectives on a topic:

- Simulation of multi-perspective debates with distinct personas and viewpoints
- Implementation of structured arguments with claims, evidence, and rebuttals
- Techniques for maintaining consistent and coherent personas throughout the debate
- Methods for handling complex, nuanced topics with multiple valid perspectives
- Prompt engineering strategies to guide the model in generating balanced arguments

### Tool Usage and Function Calling

Several notebooks demonstrate how LLMs can interact with external tools and APIs through function calling:

- Implementations of structured function schemas for API interactions
- Examples of parallel and sequential tool execution strategies
- Demonstrations of how LLMs can select appropriate tools based on user requests
- Custom tool implementations for specific domains (e.g., data analysis, web search)
- Error handling and fallback mechanisms for robust tool usage
- JSON mode for reliable structured output parsing
- Dynamic tool selection based on context

### Voice Responses and Audio Integration

The repository explores voice capabilities and audio integration with LLMs:

- Text-to-Speech (TTS) integration with OpenAI's and other providers' voice generation APIs
- Voice-based conversational interfaces with speech recognition
- Implementation of audio processing pipelines for LLM interactions
- Multi-modal applications combining text and voice for enhanced user experiences
- Examples of voice customization and styling for different applications
- Real-time voice chat implementations
- Voice character and emotion modeling
- Speech-to-text for full conversational loops

### Agent Systems

Advanced agent-based systems are demonstrated with examples of:

- Autonomous agents capable of planning and executing multi-step tasks
- Multi-agent collaboration frameworks where specialized agents work together
- Implementation of memory systems for maintaining context in long-running agents
- Problem decomposition strategies for complex tasks
- Evaluation frameworks for measuring agent performance

### Prompt Engineering Techniques

Various notebooks showcase effective prompt engineering techniques:

- Chain-of-thought prompting for complex reasoning tasks
- Few-shot learning with carefully designed examples
- System prompts for establishing constraints and behavior guidelines
- Output formatting with structured templates and parsers
- Techniques for handling ambiguity and uncertainty in user requests
- Role-based prompting with persona definitions
- Zero-shot, one-shot, and few-shot comparison analysis
- Prompt optimization and iterative refinement strategies

### Retrieval-Augmented Generation (RAG)

Implementation examples of RAG systems include:

- Document embedding and semantic search using ChromaDB and FAISS
- Knowledge base integration with different LLM providers
- Context window management for effective use of limited context
- Hybrid search techniques combining semantic and keyword-based retrieval
- Evaluation methods for measuring RAG system quality and relevance
- Query reformulation and expansion techniques
- Source attribution and citation mechanisms

## 📚 Notebook Examples

The `notebooks/` directory contains Jupyter notebooks that provide detailed examples and walkthroughs:

- `Agentic Debate.ipynb`: Implementation of a multi-turn debate system using different LLMs (GPT-4o-mini, Deepseek-R1) with Gemini as a judge
- `huggingface.ipynb`: Examples of using Hugging Face models for tasks like sentiment analysis, question answering, text summarization, and translation
- `LLM Fundamental Blocks.ipynb`: Core building blocks for LLM applications including API integrations with Azure AI Foundry, Google Gemini, and Gradio UI components
- `LLM Tools, Multi-Modality.ipynb`: Demonstrations of function calling, tool usage, image generation with DALL-E, and voice responses with TTS
- `Ollama - Email Subject Generator.ipynb`: Example of using local Ollama models to generate appropriate email subjects based on email body content
- `OpenAI - Website Summarization.ipynb`: Implementation of a website content scraper and summarizer using Azure OpenAI
- `RAG.ipynb`: Comprehensive examples of Retrieval-Augmented Generation using LangChain with ChromaDB and FAISS vector stores

Each notebook includes detailed explanations, code samples, and practical examples that you can run and modify.

## 📦 Dependencies

This project relies on several key libraries:

- **LLM Frameworks**: LangChain, OpenAI, Anthropic, Google Generative AI
- **Vector Databases**: ChromaDB, FAISS
- **ML/DL**: PyTorch, Hugging Face Transformers, Sentence Transformers
- **Visualization**: Matplotlib, Plotly
- **UI**: Gradio, JupyterLab
- **Local LLM**: Ollama
- **Audio Processing**: OpenAI TTS, PyAudio, TorchAudio

For a complete list of dependencies, see the `pyproject.toml` file.
