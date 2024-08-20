# RAG (Retrieval-Augmented Generation) com Langchain, Chroma DB, ChatGroq e TensorFlow Hub.
Este repositório contém uma implementação de um sistema RAG (Retrieval-Augmented Generation) utilizando o Langchain, Chroma DB, ChatGroq, e embeddings do TensorFlow Hub.

## Visão Geral
O RAG combina métodos de recuperação de informações com geração de texto assistida por modelos de linguagem natural. Este projeto visa criar um sistema que recupera informações relevantes de uma base de conhecimento e as utiliza para gerar respostas contextualmente relevantes a partir de um modelo de linguagem.

## Componentes Principais
* Langchain: Usado para a orquestração do pipeline de geração e recuperação, facilitando a integração dos componentes.

* Chroma DB: Banco de dados vetorial que armazena e recupera embeddings para identificar documentos relevantes.

* ChatGroq: Modelo de linguagem natural utilizado para a geração de texto, incorporando informações recuperadas.

* TensorFlow Hub: Fonte de embeddings utilizados para converter texto em vetores, que são armazenados e buscados no Chroma DB.

## Arquitetura
Pré-processamento: Os dados são processados e convertidos em embeddings usando modelos do TensorFlow Hub.
Armazenamento: Os embeddings são armazenados no Chroma DB, juntamente com os documentos de origem.
Recuperação: Dada uma consulta, os embeddings correspondentes são recuperados do Chroma DB.
Geração: O ChatGroq utiliza as informações recuperadas para gerar uma resposta contextualizada.
Requisitos
Python 3.8+
Langchain
Chroma DB
ChatGroq
TensorFlow Hub

Contribuição
Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou pull requests para melhorias ou correções.

Licença
Este projeto está licenciado sob a licença MIT. Consulte o arquivo LICENSE para mais detalhes.

