 # Product Requirements Document (PRD) || Rank your music
Mateus Neckel de Faveri || Projeto Rank your music

## 1. Visão geral e Objetivos
**Rank your music** é uma aplicação web que permite aos usuários criar e gerenciar múltiplos rankings personalizados de músicas. Como objetivo

## 2. Atores do Sistema

- **Visitante:** Usuário não autenticado que acessa a aplicação e pode visualizar rankings públicos disponibilizados pelos usuários.
- **Usuário:** Usuário autenticado que pode criar, visualizar e gerenciar seus próprios rankings, além de definir a visibilidade de cada ranking.
- **API de Músicas:** Serviço externo responsável por fornecer informações sobre as músicas pesquisadas pelo usuário, como título, artista, álbum e imagem de capa.

## 3. Histórias de usuário e Escopo

### 🔐 Épico 1: Autenticação

US01 — Criar Conta: Como um Visitante, quero criar uma conta para poder utilizar as funcionalidades de criação e gerenciamento de rankings.

Critérios de Aceitação:

- O usuário deve fornecer os dados necessários para criação da conta.
- Os campos obrigatórios devem ser validados.
- Uma conta não deve ser criada com um identificador já utilizado.

US02 — Realizar Login: Como um Usuário, quero realizar login para acessar meus rankings e funcionalidades pessoais.

Critérios de Aceitação:

- O usuário deve fornecer suas credenciais.
- Credenciais inválidas devem impedir o acesso.
- Após o login, o usuário deve ser direcionado para sua área autenticada.

US03 — Encerrar Sessão: Como um Usuário autenticado, quero encerrar minha sessão para impedir que outras pessoas utilizem minha conta no dispositivo.


### 🏆 Épico 2: Gerenciamento de Rankings

US04 — Criar Ranking: Como um Usuário, quero criar um ranking para organizar músicas de acordo com um determinado critério ou preferência.

Critérios de Aceitação:

- O ranking deve possuir um nome.
- O usuário deve ser definido como proprietário do ranking.
- O usuário deve poder definir a visibilidade do ranking como público ou privado.
- Um ranking recém-criado deve poder receber músicas.

US05 — Visualizar Meus Rankings: Como um Usuário, quero visualizar os rankings que criei para acessar e gerenciar minhas listas.

US06 — Editar Ranking: Como um Usuário, quero editar as informações de um ranking para mantê-lo atualizado.

Critérios de Aceitação:

- O proprietário deve poder alterar o nome do ranking.
- O proprietário deve poder alterar sua visibilidade.
- As alterações devem ser persistidas.

US07 — Excluir Ranking: Como um Usuário, quero excluir um ranking que não desejo mais manter.

Critérios de Aceitação:

- Somente o proprietário pode excluir o ranking.
- O sistema deve solicitar confirmação antes da exclusão.
- Após a exclusão, o ranking não deve mais aparecer entre os rankings do usuário.

### 🎶 Épico 3: Gerenciamento de Músicas

US08 — Pesquisar Música: Como um Usuário, quero pesquisar músicas por meio da aplicação para encontrar músicas que desejo adicionar aos meus rankings.

Critérios de Aceitação:

- A pesquisa deve utilizar a API externa de músicas.
- O sistema deve apresentar os resultados encontrados.
- Cada resultado deve apresentar informações suficientes para identificar a música.

US09 — Adicionar Música ao Ranking: Como um Usuário, quero adicionar uma música encontrada na pesquisa a um ranking para incluí-la na minha classificação.

Critérios de Aceitação:

- A música deve ser associada ao ranking selecionado.
- A música deve aparecer no ranking após ser adicionada.
- Uma mesma música não deve ser adicionada mais de uma vez ao mesmo ranking.

US10 — Remover Música do Ranking: Como um Usuário, quero remover uma música do ranking para alterar seu conteúdo.

US11 — Reordenar Músicas: Como um Usuário, quero alterar a posição das músicas dentro de um ranking para representar corretamente minhas preferências.

Critérios de Aceitação:

- O usuário deve poder alterar a posição de uma música.
- A ordem definida pelo usuário deve ser persistida.
- A posição das demais músicas deve ser atualizada adequadamente.
