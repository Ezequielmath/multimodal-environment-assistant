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
flowchart TD
    A["Input: Imagem do ambiente"] --> B["Visão Computacional - Detecção e Extração de Contexto"]
    B --> C["RAG - Recuperação de Conhecimento"] & E["Renderização - Visualização em Unreal Engine"]
    C --> D["Chatbot - Perguntas e Respostas Naturais"]
    D --> F["Resposta ao Usuário"]
    E --> G["Renderização Visual Interativa"]

     A:::Ash
     B:::Ash
     C:::Ash
     D:::Ash
     E:::Ash
     F:::Ash
     G:::Ash
    classDef Ash stroke-width:1px, stroke-dasharray:none, stroke:#999999, fill:#EEEEEE, color:#000000
