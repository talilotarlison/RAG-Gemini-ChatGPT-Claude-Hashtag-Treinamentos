
# RAG-Gemini-ChatGPT-Claude-Hashtag-Treinamentos

Sistema de **RAG (Retrieval-Augmented Generation)** desenvolvido em Python com interface em Streamlit, baseado no curso da Hashtag Treinamentos. O projeto demonstra como construir assistentes inteligentes utilizando diferentes modelos de linguagem:

- Google Gemini
- OpenAI ChatGPT
- Anthropic Claude

O sistema foi projetado para o setor de Recursos Humanos (RH), permitindo responder perguntas com base em informações contidas em documentos PDF.

---

## 📌 Objetivo do Projeto

Este projeto tem como objetivo mostrar como utilizar a técnica de **RAG** para consultar documentos corporativos e gerar respostas contextualizadas usando modelos de IA.

O usuário faz perguntas em linguagem natural, e o sistema:

1. Lê e processa documentos PDF;
2. Divide o conteúdo em trechos menores;
3. Gera embeddings vetoriais;
4. Armazena os vetores em um banco vetorial;
5. Recupera os trechos mais relevantes;
6. Envia o contexto para um modelo de linguagem;
7. Exibe a resposta em uma interface Streamlit.

---

## 🧠 O que é RAG?

**RAG (Retrieval-Augmented Generation)** é uma arquitetura que combina:

- **Retrieval (Recuperação):** busca trechos relevantes em documentos.
- **Generation (Geração):** utiliza um LLM para produzir respostas com base no contexto encontrado.

Essa abordagem permite respostas mais precisas e fundamentadas em dados reais da empresa.

---

## 📂 Estrutura do Projeto

O arquivo `.zip` contém três implementações independentes do mesmo sistema, cada uma utilizando um modelo diferente:

```text
RAG-Gemini-ChatGPT-Claude-Hashtag-Treinamentos/
│
├── Gemini/
│   ├── app.py
│   ├── requirements.txt
│   └── ...
│
├── ChatGPT/
│   ├── app.py
│   ├── requirements.txt
│   └── ...
│
├── Claude/
│   ├── app.py
│   ├── requirements.txt
│   └── ...
│
└── README.md
