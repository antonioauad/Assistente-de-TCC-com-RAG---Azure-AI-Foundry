
# 📘 Chat Inteligente com RAG no Azure AI Foundry para Microsoft Certification Challenge #5 - DP 100

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

Configurações e resultados do Azure Foundry
Configuração do AI HUB:

<img width="1078" height="486" alt="image" src="https://github.com/user-attachments/assets/66ebc645-2278-4ba7-bba5-8d849f78af65" />


Configuração dos modelos utilizados:

<img width="1077" height="480" alt="image" src="https://github.com/user-attachments/assets/49fb09fc-a832-404a-befa-35ada37af886" />


Execução de teste com o modelo GPT4o

<img width="1077" height="477" alt="image" src="https://github.com/user-attachments/assets/52af8cb3-1a52-4d88-9a45-4e230c9906aa" />

 
Execução de teste com o chatbot respondendo a partir dos arquivos pdf  inseridos print1:

<img width="1077" height="481" alt="image" src="https://github.com/user-attachments/assets/51e4faf9-3596-42a6-9f6b-cedb6a31c6d5" />

 
Execução de teste com o chatbot respondendo a partir dos arquivos pdf  inseridos mostrando referências :

 
<img width="1077" height="517" alt="image" src="https://github.com/user-attachments/assets/101d7507-aa13-400e-b4dd-bcd84f9d41ff" />







---

## 📁 Estrutura do Repositório

* 
`/inputs`: Contém os documentos de texto ou referências utilizadas.


* 
`README.md`: Documentação do projeto.


*Este projeto faz parte do desafio de criação de um sistema de busca inteligente para Microsoft Certification Challenge #5 - DP 100 e estudos avançados.*
