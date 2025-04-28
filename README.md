# Multimodal Environment Assistant

Um assistente virtual que analisa imagens de ambientes (ex.: salas, escritórios) usando visão computacional, responde perguntas em linguagem natural com um sistema RAG, integra um chatbot (Google Dialogflow CX), e renderiza o ambiente em Unreal Engine 5 para visualização interativa. Implementado em **Rust** com foco em prompt engineering, segurança, MLOps, e NLP.

## Objetivo
Demonstrar habilidades em:
- Rust para pipelines eficientes
- Visão computacional (ex.: YOLO)
- Retrieval-Augmented Generation (RAG) com FAISS
- Prompt engineering (few-shot, chain-of-thought)
- Chatbots com Google Dialogflow CX
- Visualização 3D com Unreal Engine 5
- Segurança e MLOps

## Stack de Tecnologias
- **Rust**: Core do projeto (tch-rs, opencv-rust, reqwest)
- **Visão Computacional**: YOLOv8, Sentence Transformers
- **RAG**: FAISS para vector database, Grok/LLaMA para LLM
- **Chatbot**: Google Dialogflow CX
- **Visualização**: Unreal Engine 5
- **NLP**: NER, topic modeling (rust-bert)
- **MLOps**: Docker, Prometheus

## Estrutura do Repositório
- `src/`: Código Rust (visão, RAG, chatbot, etc.)
- `assets/`: Imagens de teste, assets UE5
- `docs/`: Documentação (diagramas, prompts)
- `tests/`: Testes unitários
- `examples/`: Exemplos de saída

## Roadmap (8 Semanas)
- Semana 1: Planejamento, setup, repositório
- Semana 2: Visão computacional (detecção de objetos)
- Semana 3: Pipeline RAG (FAISS, LLM)
- Semana 4: Prompt engineering
- Semana 5: Chatbot (Dialogflow CX)
- Semana 6: Segurança e MLOps
- Semana 7: Unreal Engine 5
- Semana 8: NLP, testes, finalização

## Como Executar
(A ser preenchido nas próximas semanas)

## Licença
MIT License
