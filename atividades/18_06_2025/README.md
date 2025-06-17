# 📊 Análise Inteligente de Notas Fiscais

Este projeto implementa uma aplicação interativa desenvolvida com **Streamlit**, integrando **OpenAI GPT-4o** e **SQLite**, para análise inteligente de dados de notas fiscais. Os usuários podem carregar arquivos CSV de cabeçalho e itens de notas fiscais e, a partir daí, realizar perguntas em linguagem natural para obter respostas diretas ou executar consultas SQL automaticamente geradas pela IA.

---

## 🚀 Funcionalidades Principais

- **Upload de Dados CSV**  
  Permite o envio de dois arquivos CSV:
  - **Cabeçalho**: informações gerais das notas fiscais.
  - **Itens**: itens detalhados de cada nota.

- **Banco de Dados Local com SQLite**  
  Os dados carregados são armazenados em um banco SQLite temporário para consultas rápidas e estruturadas.

- **Análise Inteligente com OpenAI GPT-4o**  
  O sistema decide automaticamente:
  - Se a pergunta do usuário deve ser respondida diretamente (modo `CHAT`).
  - Ou se precisa gerar e executar uma consulta SQL (modo `SQL`).

- **Chat com Memória (via LlamaIndex ChatMemoryBuffer)**  
  O usuário pode interagir continuamente com a IA, mantendo o contexto das interações.

- **Visualização e Diagnóstico dos Dados**  
  Após o upload, o sistema exibe informações resumidas dos datasets e previews dos dados.

---

## 🛠️ Tecnologias Utilizadas

- [Streamlit](https://streamlit.io/) — Interface web interativa.
- [OpenAI GPT-4o](https://platform.openai.com/docs/) — Geração de linguagem e SQL.
- [Pandas](https://pandas.pydata.org/) — Manipulação de dados.
- [SQLite](https://www.sqlite.org/) — Banco de dados local.
- [LlamaIndex](https://llamaindex.ai/) — Memória de chat (opcional).
- [Plotly / Matplotlib / Seaborn](https://plotly.com/python/) — Visualização de dados (não totalmente habilitado no momento, mas pronto para expansão).

---

## 📦 Instalação

1️⃣ Clone o repositório:

```bash
git clone https://github.com/seu-usuario/seu-repo.git
cd seu-repo
