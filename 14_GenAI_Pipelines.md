## GenAI Pipelines

**Convolutional Neural Networks (CNNs)** are specialized deep learning models tailored for processing visual data. They utilize convolutional layers to extract features and recognize spatial patterns in images.
**Transfer learning** in CNN architecture involves utilizing pre-trained CNN models to address new image-related tasks. 

CNN architechture
1. LeNet 5,
2. AlexNet,
3. VGGNet,
4. Inception,
5. ResNet,
6. XCeption

Determinstic vs Non determinstic

Non-deterministic outputs: The same prompt can generate dozens of valid responses. Your eval system needs to assess quality across this spectrum of possibilities, not just check for exact matches.

## AI evals
#### Scope of Evaluation
1. LLM Model Evaluation
  - focuses on measuring the general language understanding of foundational LLMs using benchmark datasets eg: MMLU, _Humaneval_  
2. LLM System Evaluation
  - how well the entire application, including the LLM, performs in the context of business goals or user workflows.
https://miro.medium.com/v2/resize:fit:1400/format:webp/0*qEXafy78fJVQVk0U.png<img width="1400" height="422" alt="image" src="https://github.com/user-attachments/assets/e1219665-288e-4ef1-b959-6047ba5765eb" />

#### Common Types of Evaluation
- Hallucination
- Retrieval relevance
- Q&A on retrieved data
- Toxicity
- Summarisation performance
- Code writing correctness and readability

#### Decomposing Agent Evaluation  eg:
- Figure out which tool to call — Tool Selection eval
- Search API — Function calling eval
- Use Context — RAG eval
- Construct a response — Tone eval
- Overall Correctness — Correctness eval
