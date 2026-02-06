# 🤖 AI Data Copilot — Agent com RAG + Tools

Projeto desenvolvido para demonstrar a construção de um **AI Agent com múltiplas ferramentas**, combinando:

📚 **RAG (Retrieval-Augmented Generation)**  
🌐 **Busca Web em tempo real**  
🧮 **Execução de cálculos via Python**  
🧠 **Raciocínio ReAct (Thought → Action → Observation)**  

O objetivo é simular um **Copiloto de Dados e Operações** capaz de responder perguntas estratégicas utilizando conhecimento interno + externo.

---

## 🧭 Arquitetura do Projeto
USER QUERY
│
▼
🤖 Agent ReAct
│
├── 📚 Base RAG (Documentos internos)
├── 🌐 Busca Web (Benchmarks)
└── 🧮 Python REPL (Cálculos)
---

## 🎯 Objetivo

Construir um agente capaz de:

- Consultar bases de conhecimento corporativas  
- Buscar benchmarks de mercado em tempo real  
- Executar cálculos e simulações  
- Combinar múltiplas fontes de dados  
- Responder perguntas estratégicas de negócio  

---

## 💡 Exemplos de Perguntas

- Qual é o SLA para prioridade crítica?  
- Quando um cliente é considerado churn?  
- Qual churn médio em empresas SaaS?  
- Nosso SLA está competitivo?  
- Quanto é 15% de 1200?  

---

## 🧠 Tecnologias Utilizadas

- **LLMs (OpenAI)**
- **LangChain**
- **FAISS (Vector Store)**
- **RAG Pipeline**
- **DuckDuckGo Search**
- **Python REPL Tool**
- **ReAct Agents**

---

## 🚀 Aplicações

Este tipo de arquitetura pode ser aplicada em:

- Copilotos de Dados
- Assistentes Corporativos
- Analytics Agents
- Suporte ao Cliente
- Operações e SLA Monitoring
