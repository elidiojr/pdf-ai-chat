# Chat Interativo com PDFs usando Azure AI Foundry

Este projeto demonstra como construir um chat inteligente capaz de responder perguntas baseadas no conteúdo de arquivos PDF, utilizando o **Azure AI Foundry** – a plataforma unificada da Microsoft para desenvolvimento, customização e operação de aplicações de IA generativa e agentes inteligentes.

---

## 🚀 Visão Geral

- **Azure AI Foundry** permite criar, testar e implantar aplicações de IA generativa com facilidade, integrando modelos de ponta (OpenAI, Hugging Face, Meta, etc.) e recursos de busca vetorial para soluções robustas de RAG (Retrieval Augmented Generation).
- Combinando **Azure AI Search** e Foundry, é possível indexar documentos (como PDFs), gerar embeddings vetoriais e construir um chat que responde perguntas fundamentadas no conteúdo dos arquivos.

---

## 🛠️ Como funciona

1. **Upload de PDFs**  
   Você faz upload dos seus arquivos PDF na plataforma.

2. **Processamento e Indexação**  
   O Azure AI Foundry utiliza serviços como Azure Document Intelligence para extrair o texto dos PDFs e gerar embeddings vetoriais, que são indexados no Azure AI Search.

3. **Criação do Projeto e Deploy do Modelo**  
   - Crie um projeto no portal do Azure AI Foundry.
   - Selecione e faça o deploy de um modelo de chat (ex: GPT-4o-mini) no seu projeto.
   - Conecte o índice vetorial criado a esse modelo.

4. **Chat com seus Dados**  
   - O chat recebe perguntas do usuário.
   - A consulta é convertida em vetor e comparada com os vetores dos documentos para encontrar os trechos mais relevantes.
   - O modelo de linguagem gera uma resposta contextualizada, fundamentada nos PDFs enviados.

---

## 💡 Exemplos de Uso

- **Pergunta:** "Quais são as vantagens do uso de busca vetorial em sistemas de informação?"
- **Resposta do chat:** "Segundo o artigo X, a busca vetorial permite encontrar informações similares mesmo quando os termos exatos não são usados, melhorando a precisão em grandes volumes de dados."

---

## ✨ O que aprendi e possibilidades

- **Facilidade de integração:** O Azure AI Foundry centraliza ferramentas para processamento de documentos, criação de índices vetoriais e integração com modelos generativos, tornando o desenvolvimento mais ágil e seguro.
- **RAG na prática:** É possível criar facilmente soluções de RAG, onde o modelo de IA responde com base nos seus próprios dados, não só no conhecimento pré-treinado.
- **Expansão:** O mesmo fluxo pode ser usado para outros tipos de documentos e integrações, inclusive com múltiplos modelos e fontes de dados.
- **Governança e segurança:** A plataforma oferece recursos de monitoramento, controle de acesso e compliance para uso corporativo.




