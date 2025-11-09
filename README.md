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
