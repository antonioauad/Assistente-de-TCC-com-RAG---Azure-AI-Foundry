
# 📘 Chat Inteligente com RAG no Azure AI Foundry

Este projeto consiste na criação de um assistente virtual personalizado que utiliza a técnica de **RAG (Retrieval-Augmented Generation)** para responder perguntas baseadas em documentos PDF específicos.

## 🚀 Tecnologias Utilizadas

* 
**Azure AI Foundry** 


* 
**Azure OpenAI** (Modelos GPT e Embeddings) 


* 
**Azure AI Search** (Busca Vetorial) 


* **Python** (Opcional para integração)

## 🛠️ Passo a Passo da Implementação

### 1. Configuração do Ambiente no Azure 🏗️

* Acesse o portal do [Azure AI Foundry](https://ai.azure.com/).
* Crie um novo **Projeto** e vincule um recurso do **Azure OpenAI**.
* Certifique-se de ter um recurso do **Azure AI Search** disponível na mesma região para indexação.

### 2. Implantação de Modelos 🤖

* Vá em **Deployments** e implemente dois modelos essenciais:
* **Modelo de Chat**: Ex: `gpt-35-turbo` ou `gpt-4`.
* **Modelo de Embeddings**: Ex: `text-embedding-3-small` (necessário para transformar texto em vetores).



### 3. Importação e Vetorização de Dados (Ingestion) 📁

* No menu lateral, selecione **Data + Indexes**.
* Clique em **+ New Index** e escolha a fonte de dados (Upload de arquivos PDF).


* Suba os seus artigos científicos ou documentos na pasta `inputs`.


* Configure a tarefa de ingestão para utilizar o modelo de **embeddings** implantado. Isso criará uma base de dados vetorial no Azure AI Search.



### 4. Criação do Playground de Chat 💬

* Acesse o **Playground**.
* No painel de configuração, em "Add your data", selecione o índice que você acabou de criar.


* Configure os parâmetros de sistema (System Message) para definir como o assistente deve se comportar.

### 5. Testes e Refinamento 🧪

* Realize perguntas no chat interativo para validar se as respostas estão sendo fundamentadas nos PDFs carregados.


* Verifique as citações para garantir que a IA está localizando a informação correta nos documentos.



---

## 📈 Insights Aprendidos

* 
**Eficiência na Busca**: A busca vetorial permite encontrar contextos que palavras-chave simples ignorariam.


* 
**Redução de Alucinações**: Ao limitar a IA ao conteúdo dos documentos (RAG), as respostas tornam-se muito mais precisas e confiáveis.


* 
**Escalabilidade**: O sistema pode processar centenas de documentos, facilitando a vida de estudantes e pesquisadores.



---

## 📁 Estrutura do Repositório

* 
`/inputs`: Contém os documentos de texto ou referências utilizadas.


* 
`README.md`: Documentação do projeto.


*Este projeto faz parte do desafio de criação de um sistema de busca inteligente para TCC e estudos avançados.*
