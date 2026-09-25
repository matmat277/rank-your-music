# 🎶Rank-your-music🎶
Website de listagem de músicas por ordem de preferência própria do usuário.


## Autor: Mateus Neckel de Faveri

O frontend da aplicação foi desenvolvido com HTML, CSS e JavaScript e o backend foi simulado pela implementação de uma API Fake, usando o JSON Server.

## 📚 Documentação do Projeto
Para entender as regras de negócio, o escopo e a arquitetura técnica da aplicação, consulte os documentos abaixo:

## 📄 Product Requirements Document (PRD) - Visão geral, atores e histórias de usuário.
- [🛠️ Especificação Técnica (PRD)](https://github.com/matmat277/rank-your-music/blob/main/docs/prd.md)
- [Arquitetura do sistema (architecture)](https://github.com/matmat277/rank-your-music/blob/main/docs/architecture.md)

# 🎨 Design 

🎨 Design System - Identidade visual

🖼️ Protótipo no Figma - [Telas interativas da aplicação.](https://www.figma.com/proto/nHBtWB00QHD7x9OkE3OnWS/Rank-your-music?node-id=8-412&t=KHuAm6fWMQ7R8NZ1-0&scaling=min-zoom&content-scaling=fixed&page-id=0%3A1&starting-point-node-id=8%3A412&show-proto-sidebar=1&fuid=1500934227224952569)

🌐 Site em Produção - GitHub Pages


## 💻 Tecnologias e Dependências
 - Framework CSS: Bootstrap (Grid responsivo, utilitários de layout e componentes JS nativos, além de ser o framework mais usado do mundo).
 - Preprocessador CSS: SaSS/SCSS (Escolhido para modularizar o CSS e sobreescrever as variáveis nativas do bootstrap, permitindo aplcar fielmente o design desenhado no Figma).
 - JavaScript: ES6+ Vanilla JS + jQuery (Utilizads em conjunto para a manipulação dinâmica do DOM, controle de fluxo do formulário multi-etapas, gerenciamento de modais e requisições assincronas).
 - API Fake Local: JSON server (Empregado como API Fake local para simular a persistência de dados dos cadastros de usuários e suas preferências táticas na coleção `user`).
 - API externa pública: MusicBrainz + Cover art Archive (API para coleta de dados ou informações sobre as músicas requisitadas, cover art é parte da API de MusicBrainz que somente localiza imagem do álbum/música).


## ✅ Checklist | Indicadores de Desempenho (ID) dos Resultados de Aprendizagem (RA)

#### RA1 - Utilizar Frameworks CSS para estilização de elementos HTML e criação de layouts responsivos.

- [ ] ID 01 - Prototipa interfaces adaptáveis para no mínimo os tamanhos de tela mobile e desktop, usando ferramentas de design tradicionais (Figma, Quant UX ou Sketch) ou IA (Stitch).
- [ ] ID 02 - Implementa layout responsivo com Framework CSS (Bootstrap, Materialize, Tailwind + DaisyUI) usando Flexbox ou Grid do próprio framework.
- [ ] ID 03 - Implementa layout responsivo com CSS puro, usando Flexbox ou Grid Layout.
- [ ] ID 04 - Utiliza componentes prontos de um Framework CSS (ex.: card, button) e componentes JavaScript do framework (ex.: modal, carousel).
- [ ] ID 05 - Cria layout fluido usando unidades relativas (vw, vh, %, em, rem) no lugar de unidades fixas (px).
- [ ] ID 06 - Aplica um Design System consistente (cores, tipografia, padrões de componentes) em toda a aplicação.
- [ ] ID 07 - Utiliza Sass (SCSS) com ou sem framework, aplicando variáveis, mixins e funções para modularizar o código.
- [ ] ID 08 - Aplica tipografia responsiva (media queries mobile first) ou tipografia fluida (função clamp() + unidades relativas).
- [ ] ID 09 - Aplica técnicas de responsividade de imagens usando CSS (object-fit, containers com unidades relativas).
- [ ] ID 10 - Otimiza imagens usando formatos modernos (WebP) e carregamento adaptativo (srcset, picture, ou parâmetros do Cloudinary).

#### RA2 - Realizar tratamento de formulários e aplicar validações customizadas no lado cliente.

- [ ] ID 11 - Implementa validação HTML nativa (campos obrigatórios, tipos, limites de caracteres) com mensagens de erro/sucesso no lado cliente.
- [ ] ID 12 - Aplica expressões regulares (REGEX) para validações customizadas (e-mail, telefone, datas, etc.)
- [ ] ID 13 - Utiliza elementos de seleção em formulários (checkbox, radio, select) para coleta de dados.
- [ ] ID 14 - Implementa leitura e escrita no Web Storage (localStorage/sessionStorage) para persistir dados localmente.

#### RA3 - Aplicar ferramentas para otimização do processo de desenvolvimento web.

- [x] ID 15 - Configura ambiente com Node.js e NPM para gerenciamento de pacotes e dependências.
- [x] ID 16 - Utiliza boas práticas de versionamento no Git/GitHub (branch main ou branches específicos, uso de .gitignore).
- [x] ID 17 - Mantém um README.md padronizado, conforme template da disciplina, com checklist preenchido.
- [x] ID 18 - Organiza arquivos do projeto de forma modular, seguindo padrão de exemplo fornecido.
- [x] ID 19 - Configura linters e formatadores (ESLint, Prettier) para manter qualidade e padronização do código.

#### RA4 - Aplicar bibliotecas de funções e componentes em JavaScript para aprimorar a interatividade de páginas web.

- [ ] ID 20 - Utiliza jQuery para manipulação do DOM e interatividade (eventos, animações, manipulação de elementos)
- [ ] ID 21 - Integra e configura um plugin jQuery relevante (ex.: jQuery Mask Plugin).

#### RA5 - Efetuar requisições assíncronas para uma API fake e APIs públicas, permitindo a obtenção e manipulação de dados dinamicamente.

- [ ] ID 22 - Realiza requisições assíncronas para uma API fake (ex.: JSON Server) para persistir dados de um formulário.
- [ ] ID 23 - Realiza requisições assíncronas para uma API fake para exibir dados na página.
- [ ] ID 24 - Realiza requisições assíncronas para APIs públicas reais (OpenWeather, ViaCEP etc.), exibindo os dados e tratando erros.
