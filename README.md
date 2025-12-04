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
# Prints do trabalho

- Workflow completo
  <img width="1132" height="710" alt="image" src="https://github.com/user-attachments/assets/70696038-1857-4861-8c16-4dcf0532a1f7" />

- Print da database no supabase
  <img width="1872" height="932" alt="image" src="https://github.com/user-attachments/assets/cf58d6f5-ff43-4220-80c3-4637b63c926d" />

  <img width="1570" height="774" alt="image" src="https://github.com/user-attachments/assets/f7557bd4-112e-4549-9cb1-477c3b048f7c" />
