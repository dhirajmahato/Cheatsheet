
# Transformers
Theses are neural network architectures that rely heavily on **self-attention mechanisms** to model relationships between **tokens in sequences**.
## Types based on design architecture and purpose.
1. **Encoder only**
Great at understanding text (classification, embedding, etc.).
  - BERT (Bidirectional Encoder Representations from Transformers)
  - RoBERTa (Robustly optimized BERT)
  - DistilBERT (smaller and faster BERT)
  - ALBERT (lite BERT with parameter sharing)
2. **Decoder only**
Great for text generation (autogressive tasks).
  - GPT (Generative Pretrained Transformer) family: GPT-2, GPT-3, GPT-4, GPT-4.5
  - LLaMA (Meta’s series) – designed to be efficient
  - Mistral, Grok (by xAI), Falcon – decoder-style, optimized for performance
3. **Encoder- Decoder Transformers**
Suited for translation, summarization, question-answering.
  - T5 (Text-to-Text Transfer Transformer)
  - BART (Bidirectional and Auto-Regressive Transformer)
  - mT5, MBART (multilingual variants)

_ADVANCED VARIATIONS & ARCHITECTURAL INNOVATIONS_

4. **Sparse Models / Mixture of Experts (MoE)**
Only a subset of parameters are active per forward pass.
  - Improves compute efficiency.
  - Examples: Mixtral, GShard, Switch Transformer

5. **Retrieval-Augmented Generation (RAG)**
Combines transformer with external knowledge (e.g., vector DB).
  - Useful in enterprise knowledge applications.
  - Examples: GPT with RAG, Command R+, LLamaIndex setups

6. **Long-context Transformers**
Standard transformers scale poorly with long sequences.
  - Solutions include: sliding windows, recurrence, sparse attention.
  - Examples:Claude 3.5: Handles 200k+ tokens; Gemini 1.5 Pro: 1M context window, Longformer, BigBird, FlashAttention, RWKV

## Usecases 

| Task                                 | Best Model Type                |
| ------------------------------------ | ------------------------------ |
| Sentiment analysis, intent detection | Encoder-only (BERT)            |
| Text generation, chatbot             | Decoder-only (GPT, LLaMA)      |
| Translation, summarization           | Encoder-decoder (T5, BART)     |
| Document Q\&A (RAG)                  | Decoder with retrieval         |
| Multimodal Q\&A                      | GPT-4-Vision, Gemini           |
| Domain-specific LLM                  | Fine-tuned LLaMA, Mistral, GPT |


# LLMs
LLMs are **trained transformer-based models** with billions of parameters. They're categorized based on openness, size, fine-tuning capability, and architecture.


