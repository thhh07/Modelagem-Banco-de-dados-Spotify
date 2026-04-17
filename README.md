# Modelagem-Banco-de-dados-Spotify
Teste de banco de dados do Spotify
🎧 Modelo Entidade-Relacionamento - Spotify

Este repositório apresenta um modelo de banco de dados baseado no funcionamento do Spotify, utilizando o paradigma de Entidade-Relacionamento (ER). O objetivo é representar de forma simplificada como músicas, artistas, usuários e playlists se relacionam dentro da plataforma.

📌 Entidades principais
Usuário (User)
Representa os usuários da plataforma.
Atributos: id, nome, email, data_criacao, tipo_conta
Artista (Artist)
Representa artistas ou bandas.
Atributos: id, nome, genero
Álbum (Album)
Conjunto de músicas lançadas por um artista.
Atributos: id, titulo, data_lancamento
Música (Track)
Representa as faixas disponíveis na plataforma.
Atributos: id, titulo, duracao, popularidade
Playlist (Playlist)
Coleção de músicas criada por usuários.
Atributos: id, nome, data_criacao, privada
🔗 Relacionamentos
Usuário cria Playlist
Um usuário pode criar várias playlists (1:N)
Playlist contém Música
Uma playlist pode conter várias músicas e uma música pode estar em várias playlists (N:N)
Artista lança Álbum
Um artista pode lançar vários álbuns (1:N)
Álbum contém Música
Um álbum possui várias músicas (1:N)
Usuário escuta Música
Representa o histórico de reprodução (N:N), podendo incluir atributos como data_execucao
