# Projeto RAG Híbrida - Sistema de IA com Busca Vetorial

Sistema de Retrieval-Augmented Generation (RAG) híbrido implementado no n8n que combina processamento de linguagem natural com busca vectorial para consulta inteligente de dados.

link do video: https://youtu.be/rsqoKGVAYpI

## ✨ Funcionalidades

- **Chatbot Inteligente**: Interface conversacional com capacidade de memória contextual
- **Busca Híbrida**: Combina busca vectorial semântica com filtros tradicionais
- **Integração Multi-fonte**: Conexão com Google Sheets, Supabase e APIs externas
- **Processamento de Documentos**: Carregamento, divisão e vetorização de dados estruturados
- **Armazenamento Vectorial**: Indexação e busca semântica no Supabase Vector Store
- **Pipeline ETL**: Extração, transformação e carga de dados de planilhas para vector store

## 🛠️ Tecnologias Utilizadas

### Núcleo do Sistema
- **n8n** - Plataforma de automação e orquestração
- **Supabase** - Banco de dados + Vector Store
- **OpenAI** - Modelos de linguagem e embeddings
- **Google Sheets** - Fonte de dados principal

### Integrações e APIs
- **@n8n/n8n-nodes-langchain** - Integração com LangChain
- **HTTP Request Tool** - Comunicação com APIs externas
- **Custom Functions** - Busca híbrida personalizada

## 🏗️ Arquitetura do Workflow

### Fluxo de Carregamento (ETL)

```
Manual Trigger → Google Sheets → Transformação →
Text Processing → Vector Store → Supabase
```
### Fluxo de Consulta (Chat)
```
Chat Trigger → AI Agent → OpenAI →
Memory → Hybrid Search → Response
```
