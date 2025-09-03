Título: Desafio backend-br - Encurtador de URLs 

Descrição: 
(contato)
(link do desafio)
(link para o GitHub da solução)
(links das documentações das ferramentas utilizadas)

### Introdução

- [ ] Apresentação
- [ ] Leitura do desafio
- [ ] Tecnologias utilizadas

### back-end

- [x] Iniciar Projeto bun;

``` shell
bun init
```

- [ ] Instalar as dependências;

``` shell
bun add fastify
bun add redis
```

- [ ] Configuração base do servidor;
- [ ] onfigurar Docker para rodar o Redis;

``` yml
services:
  redis:
    image: redis
    container_name: redis
    command: redis-server --requirepass Redis2019!
    ports:
      - "6379:6379"
```

- [ ] \[POST] - rota para encurtar URL;
- [ ] \[GET] - rota para acessar URL;
	- [ ] Definir TTL (Time to live) - seconds

### front-end

- [ ] Importar base do front-end;
- [ ] Modificar o servidor para entregar o front-end;
- [ ] Formulário para gerar a URL encurtada;
- [ ] Janela para exibição do anúncio, e redirecionamento

### Encerramento 

- [ ] Possíveis evoluções para o projeto
	- Personalização da URLs curta.
	- Interface para gestão dos links criados (CRUD)
	- Autenticação
	- Implementação de métricas
		- Número total de cliques
		- Cliques únicos
		- Origem dos clicks: (Geolocalização, Navegador, SO)
		- Horários dos acessos

- [ ] Conclusão


API de Geolocalização: http://ip-api.com/json