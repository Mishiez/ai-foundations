# AI Foundations

A small, checkpointed learning project covering the AI landscape, LLM fundamentals, and a first Gemini API request from Python.

## Contents

- [AI landscape](ai-landscape.md): relationships among AI, machine learning, deep learning, NLP, computer vision, and generative AI.
- [LLM fundamentals](ai-landscape.md#llm-fundamentals): tokens, tokenization, embeddings, transformers, attention, and context windows.
- [Gemini API notebook](h1_llm_api_demo.ipynb): loads an API key securely, creates a Gemini client, and prints a generated response.

## Setup

From the repository root, create and activate a virtual environment:

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

Create a local `.env` file from `.env.example` and replace the placeholder with a Gemini API key:

```text
GEMINI_API_KEY=your_key_here
```

Keep `.env` private. It is ignored by Git. Never paste the key into the notebook or commit it to the repository.

## Run the Notebook

Open `h1_llm_api_demo.ipynb` in VS Code, select the `.venv` Python kernel, and run the cells from top to bottom. The key-loading cell should report that the key was loaded, and the final cell prints the generated explanation of machine learning.

The notebook uses the Google Gemini Python SDK and the `gemini-3.6-flash` model. Model availability and free-tier limits depend on the Google account and API project associated with the key.
