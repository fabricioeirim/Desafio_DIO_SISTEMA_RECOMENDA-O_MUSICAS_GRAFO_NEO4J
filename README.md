Detalhes da criação dos scripts e estrutura do sistema de reocmendação.

🎼 1. Estrutura do Grafo
Nódulos (Nodes):
Usuario: nome, email, idade

Artista: nome, gênero

Musica: título, duração

Genero: nome

Relacionamentos (Edges):
(:Usuario)-[:OUVIU {vezes, ultimaVez}]->(:Musica)

(:Usuario)-[:CURTIU]->(:Musica)

(:Usuario)-[:SEGUE]->(:Artista)

(:Artista)-[:CANTA]->(:Musica)

(:Musica)-[:PERTENCE_A]->(:Genero)

<img width="1285" height="877" alt="image" src="https://github.com/user-attachments/assets/93f864c7-b9d5-468f-bdd9-45e7b23ffdf9" />
