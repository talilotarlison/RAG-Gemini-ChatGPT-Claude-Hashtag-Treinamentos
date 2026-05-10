
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
````

---

## 🤖 Modelos Utilizados

### 🔹 Google Gemini

Implementação utilizando a API do Google Gemini.

### 🔹 OpenAI ChatGPT

Implementação utilizando modelos GPT da OpenAI.

### 🔹 Anthropic Claude

Implementação utilizando a API da Anthropic.

---

## 🛠️ Tecnologias Utilizadas

* Python 3.10+
* Streamlit
* LangChain
* FAISS ou ChromaDB
* PyPDF2 ou pypdf
* Embeddings
* APIs:

  * Google Gemini
  * OpenAI
  * Anthropic

---

## 📄 Funcionalidades

* Upload de arquivos PDF
* Extração de texto
* Segmentação em chunks
* Geração de embeddings
* Armazenamento vetorial
* Busca semântica
* Respostas com base no documento
* Interface web com Streamlit
* Suporte a múltiplos provedores de IA

---

## 🚀 Instalação

### 1. Clone o repositório

```bash
git clone <url-do-repositorio>
cd RAG-Gemini-ChatGPT-Claude-Hashtag-Treinamentos
```

### 2. Escolha um dos projetos

```bash
cd ChatGPT
# ou
cd Gemini
# ou
cd Claude
```

### 3. Crie um ambiente virtual

```bash
python -m venv .venv
```

### 4. Ative o ambiente virtual

#### Windows

```bash
.venv\Scripts\activate
```

#### Linux/Mac

```bash
source .venv/bin/activate
```

### 5. Instale as dependências

```bash
pip install -r requirements.txt
```

---

## 🔑 Configuração das Chaves de API

Crie um arquivo `.env` com a chave correspondente ao modelo escolhido.

### OpenAI

```env
OPENAI_API_KEY=sua_chave_aqui
```

### Google Gemini

```env
GOOGLE_API_KEY=sua_chave_aqui
```

### Anthropic Claude

```env
ANTHROPIC_API_KEY=sua_chave_aqui
```

---

## ▶️ Execução

```bash
streamlit run app.py
```

A aplicação será aberta automaticamente no navegador.

---

## 🧑‍💼 Caso de Uso: Assistente de RH

O sistema foi desenvolvido como um assistente virtual para Recursos Humanos.

### Exemplos de perguntas:

* "Quantos dias de férias o colaborador tem direito?"
* "Qual é a política de home office?"
* "Como funciona o banco de horas?"
* "Quais benefícios são oferecidos pela empresa?"
* "Qual o prazo para solicitar reembolso?"

O sistema consulta o PDF da empresa e responde com base nas informações encontradas.

---

## 📘 Fluxo do Sistema

```text
PDF → Extração de Texto → Chunks → Embeddings → Banco Vetorial
     → Busca Semântica → Contexto → LLM → Resposta
```

---

## 📸 Interface

A aplicação em Streamlit permite:

* Upload do PDF
* Campo para digitar perguntas
* Visualização das respostas em tempo real

---

## 🔍 Exemplo de Uso

1. Execute a aplicação.
2. Faça upload do manual ou política em PDF.
3. Digite uma pergunta.
4. Receba uma resposta fundamentada no documento.

---

## 📈 Melhorias Futuras

* Upload de múltiplos documentos
* Histórico de conversas
* Citação das páginas do PDF
* Exportação das respostas
* Controle de acesso
* Deploy em nuvem

---

## 🎓 Créditos

Projeto desenvolvido com base no curso da Hashtag Treinamentos.

[Hashtag Treinamentos](https://www.hashtagtreinamentos.com?utm_source=chatgpt.com)

---

## 📄 Licença

Este projeto é destinado a fins educacionais e de aprendizado.

```

