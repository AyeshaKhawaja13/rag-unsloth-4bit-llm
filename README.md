Retrieval-Augmented Generation (RAG) with Unsloth 4-bit Quantized LLM
 Overview

This project implements a Retrieval-Augmented Generation (RAG) pipeline using a dynamically quantized 4-bit LLM from Unsloth. The system retrieves relevant document chunks using FAISS vector search and generates grounded responses using a memory-efficient LLM.

The project is optimized for low VRAM environments (Google Colab T4 GPU).

Architecture

User Query
   ↓
Vector Retrieval (FAISS)
   ↓
Relevant Context Chunks
   ↓
4-bit Quantized LLM (Unsloth)
   ↓
Grounded Response

Technologies Used

- Unsloth (Dynamic 4-bit Quantization)
- Transformers
- FAISS (Vector Store)
- SentenceTransformers (Embeddings)
- PyTorch
- Google Colab (GPU)

Key Features

- Dynamic 4-bit model loading for optimal VRAM usage
- Efficient document chunking
- FAISS-based similarity search
- Prompt-engineered grounded generation
- End-to-end RAG pipeline

Model Used

- unsloth/Qwen2.5-7B-Instruct-bnb-4bit

Results

- Reduced GPU memory usage using 4-bit quantization
- Accurate retrieval-grounded responses
- Stable inference on T4 GPU

How to Run

1. Open the notebook in Google Colab
2. Enable GPU runtime
3. Install dependencies
4. Run all cells sequentially

Future Improvements

- Add PDF ingestion
- Streamlit interface
- Evaluation metrics (RAGAS)
- Deploy as API

Author

Ayesha Shafique
BSCS | AI/ML Developer
