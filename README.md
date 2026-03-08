# Assistente-de-TCC-com-RAG---Azure-AI-Foundry

Visão Geral:
"Este projeto implementa um sistema de Recuperação Aumentada por Geração (RAG) utilizando o Azure AI Foundry. O objetivo é permitir que estudantes de Engenharia de Software consultem bases extensas de PDFs (Artigos Científicos) de forma intuitiva e fundamentada."

Insights Técnicos:

Segurança Corporativa: Diferente de IAs públicas, o uso do Azure garante que os documentos do TCC não sejam usados para treinar modelos globais.

Busca Híbrida: No Azure AI Search, utilizei busca semântica + vetorial para garantir que, mesmo que o usuário use termos diferentes dos artigos, a IA encontre o contexto correto.

Prompt Engineering: Ajustei o System Message para que a IA cite explicitamente qual PDF foi usado para gerar a resposta.
