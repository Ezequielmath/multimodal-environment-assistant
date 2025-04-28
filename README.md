# Multimodal Environment Assistant

Um assistente virtual que analisa imagens de ambientes (ex.: salas, escritórios) usando visão computacional, responde perguntas em linguagem natural com um sistema RAG, integra um chatbot (Google Dialogflow CX), e renderiza o ambiente em Unreal Engine 5. Implementado em **Rust** com foco em prompt engineering, segurança, MLOps, e NLP.

## Objetivo
Demonstrar habilidades em Rust, visão computacional, RAG, chatbots, e visualização 3D para aplicações de IA multimodal.

## Stack de Tecnologias
- **Rust**: Core do projeto (tch-rs, reqwest, serde)
- **Visão Computacional**: YOLOv8, Sentence Transformers
- **RAG**: FAISS, Grok/LLaMA
- **Chatbot**: Google Dialogflow CX
- **Visualização**: Unreal Engine 5
- **MLOps**: Docker, Prometheus

## Arquitetura
```mermaid
graph TD
    A[Input Image] --> B[Vision Model (YOLO)]
    B --> C[Text Descriptions]
    C --> D[Embeddings (Sentence Transformers)]
    D --> E[Vector Database (FAISS)]
    E --> F[LLM (Grok/LLaMA)]
    F --> G[Chatbot (Dialogflow CX)]
    G --> H[Web Interface]
    C --> I[Unreal Engine 5 (3D Render)]
    F --> I
