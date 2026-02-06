# 🤖 AI Data Copilot — Agent com RAG + Tools

Projeto desenvolvido para demonstrar a construção de um **AI Agent com múltiplas ferramentas**, combinando:

📚 **RAG (Retrieval-Augmented Generation)**  
🌐 **Busca Web em tempo real**  
🧮 **Execução de cálculos via Python**  
🧠 **Raciocínio ReAct (Thought → Action → Observation)**  

O objetivo é simular um **Copiloto de Dados e Operações** capaz de responder perguntas estratégicas utilizando conhecimento interno + externo.

---

# 🎯 Objetivo

Construir um agente capaz de responder perguntas como:

- "Qual é o SLA para prioridade crítica?"
- "Qual churn médio em empresas SaaS?"
- "Nosso SLA está competitivo?"
- "Quanto é 15% de 1200?"

Utilizando automaticamente a ferramenta correta.

---

# 🧱 Pipeline do Projeto

## 1️⃣ Carregamento de Documentos

Documentos internos utilizados como base de conhecimento:

- Políticas de SLA  
- Definições de churn  
- Processos de suporte  
- Indicadores operacionais  

**Formatos suportados:**

- TXT  
- PDF  

---

## 2️⃣ Chunking

Divisão dos documentos em partes menores para melhorar recuperação semântica.

**Configuração utilizada:**

chunk_size = 400
chunk_overlap = 100

---

## 3️⃣ Embeddings

Transformação dos textos em vetores semânticos utilizando OpenAI Embeddings.

Isso permite:

- Busca contextual  
- Similaridade semântica  
- Recuperação precisa  

---

## 4️⃣ Vector Store (FAISS)

Indexação vetorial com FAISS para recuperação eficiente.

**Recursos:**

- Armazenamento local  
- Cache de embeddings  
- Carregamento rápido  

---

## 5️⃣ Retriever

Responsável por localizar os chunks mais relevantes para cada pergunta.

**Exemplo:**

Pergunta → "SLA prioridade crítica"

Retriever → Busca trechos sobre SLA crítico.

---

## 6️⃣ QA Chain (RAG)

Combina:

- Contexto recuperado  
- Prompt template  
- LLM  

Para gerar respostas fundamentadas.

---

# 🧰 Tools do Agent

O Agent possui acesso a três ferramentas principais.

---

## 📚 1) Base de Conhecimento (RAG)

Consulta documentos internos da empresa.

Utilizada para:

- Políticas de SLA  
- Definições de churn  
- Processos operacionais  

---

## 🌐 2) Busca Web

Integração com DuckDuckGo.

Utilizada para:

- Benchmarks de mercado  
- Métricas SaaS  
- Boas práticas  

---

## 🧮 3) Python REPL

Permite execução de código Python.

Utilizada para:

- Cálculos percentuais  
- Simulações  
- Análises numéricas  

---

# 🤖 Criação do Agent

O Agent foi construído utilizando arquitetura **ReAct**.

**Fluxo de raciocínio:**

Thought → Action → Observation → Final Answer

Isso permite que o modelo:

- Pense no que fazer  
- Escolha a tool  
- Execute a ação  
- Use o resultado na resposta  

---

# 🧪 Testes Realizados

Os testes foram organizados por categoria.

---

## 📚 RAG

- Qual é o SLA para prioridade crítica?  
- Quando um cliente é considerado churn?  

---

## 🌐 Web

- Qual é o churn médio em empresas SaaS?  
- Quais são as melhores práticas de SLA?  

---

## 🧮 Python

- Qual é 15% de 1200?  
- Se 8% de 500 tickets estão fora do SLA, quantos são?  

---

## 🔀 Multi-Tools

- Nosso SLA está competitivo comparado ao mercado?  
- Como reduzir churn mantendo SLA saudável?  

---

# 🧠 Exemplo de Reasoning

Thought: Preciso consultar políticas internas
Action: Base de Conhecimento
Observation: SLA crítico = 24h
Final Answer: O SLA é de até 24 horas

---

# 🛠️ Stack Tecnológica

- LangChain  
- OpenAI  
- FAISS  
- DuckDuckGo Search  
- Python REPL  
- Jupyter Notebook  

---

# 🚀 Possíveis Evoluções

- Streamlit UI  
- SQL Tool  
- Memory  
- Multi-Agent  
- Avaliação de grounding RAG  

---

# 📌 Conclusão

Este projeto demonstra a construção completa de um **AI Agent com RAG e múltiplas ferramentas**, capaz de:

- Integrar conhecimento interno  
- Consultar dados externos  
- Executar cálculos  
- Raciocinar em múltiplos passos  

Representa uma aplicação prática de Agents para cenários de negócio e dados.

---

# 👨‍💻 Autor

Projeto desenvolvido para fins de estudo e portfólio em IA, Dados e LLM Engineering.

---

⭐ Se este projeto foi útil, considere dar uma estrela no repositório.
