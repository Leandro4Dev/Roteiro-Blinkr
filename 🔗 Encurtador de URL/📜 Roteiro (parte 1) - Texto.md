
### Introdução

Fala galera, eu sou o Leandro.

No vídeo de hoje, vamos resolver juntos um desafio de back-end, proposto pela galera da página backend-br. 

Como vocês já viram no título do vídeo, o desafio proposto é um encurtador de URLs.

Como um extra nesse vídeo também vamos implementar um front-end simples com o formulário para encurtar as URLs e também uma página para exibir anúncios antes do redirecionamento.

Então chega de enrolação, e vamos para o repositório do desafio, para entender os requisitos

(Leitura do desafio)

Neste projeto eu decide utilizar o TypeScript com o fastify, rodando no bun para simplificar.

Para armazenar as URLs vamos utilizar o Redis como armazenamento de chave valor.
porque ele já faz o gerenciamento do tempo de vida dos registros automaticamente. então não vamos precisar implementar essa parte no código.

E para rodar o Redis eu vou utilizar o Docker.

Então vamos para o código!!

Eu criei uma lista para separa os passos que vamos seguir.

(Abrir o Obsidian e mostrar a lista)

Primeiramente, vamos iniciar o projeto e instalar as dependências.

(Enquanto as dependências são instaladas) Galera eu estou partindo do princípio, que vocês já tenham  as ferramentas que eu citei instaladas na máquina de vocês, não vou me aprofundar em como fazer a instalação de cada uma delas, mas vou deixar o links das documentações oficiais na descrição.