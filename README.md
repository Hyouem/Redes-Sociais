# Redes-Sociais
Redes-Sociais
Escopo do Projeto

Este projeto tem como foco a análise de dados de redes sociais utilizando banco de dados orientado a grafos, com ênfase no Neo4j e na linguagem de consulta Cypher. A proposta é demonstrar como a modelagem em grafos permite representar de forma eficiente usuários, conteúdos e interações, explorando relacionamentos complexos e consultas avançadas.

Objetivos

Modelar dados de redes sociais utilizando nós, relacionamentos e propriedades no Neo4j;

Aplicar consultas Cypher para análise de conexões, interações e padrões de engajamento;

Explorar relacionamentos diretos e indiretos entre usuários;

Identificar usuários influentes com base em grau de relacionamento e interações;

Demonstrar boas práticas de criação e uso de índices e constraints para otimização de consultas.

Modelagem de Dados

O modelo de grafos contempla entidades como:

Usuário (User)

Postagem (Post)

Comentário (Comment)

Hashtag (Hashtag)

E relacionamentos como:

(:User)-[:FOLLOWS]->(:User)

(:User)-[:POSTS]->(:Post)

(:User)-[:LIKES]->(:Post)

(:User)-[:COMMENTS]->(:Comment)

(:Post)-[:HAS_HASHTAG]->(:Hashtag)

Essa modelagem facilita consultas que exploram profundidade, vizinhança e padrões de interação.

Consultas Cypher

O projeto inclui consultas Cypher para:

Buscar usuários com maior número de conexões e interações;

Identificar comunidades de usuários por meio de padrões de relacionamento;

Analisar engajamento em postagens específicas;

Explorar caminhos entre usuários (ex: conexões de segundo e terceiro nível);

Avaliar desempenho de consultas utilizando índices e filtros por propriedades.

Tecnologias Utilizadas

Neo4j

Cypher Query Language

Neo4j Browser / Neo4j Desktop

Dataset fictício para fins educacionais
