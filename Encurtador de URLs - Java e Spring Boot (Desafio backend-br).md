
Fala galera blz!?

### Introdução
Nesse vídeo vamos resolver um desfio de código que encontrei no repositório da comunidade "backend.br".

A ideia central do desafio é bem simples, mas no final vamos "incrementar" um pouco a solução. 

Então vamos abrir a repositório do desafio para entender os requisitos.
### Lendo desafio

Vamos lá, 
"Seu desafio será implementar um serviço que permite encurtar URLs longas para torná-las mais compactas e fáceis de compartilhar."

Então ele nos mostra um exemplo de uma rota POST que recebe no seu body um json com a propriedade "url". E retorna um json com a url encurtada.

Com eu falei a ideia é bem simples.

Ele também vai especificar alguns requisitos, vamos ver quais são:

primeiro,
"O encurtador de URLs recebe uma URL longa como parâmetro inicial."
certo isso ai já é padrão, como vimos no exemplo.

segundo,
"O encurtamento será composto por um mínimo de 05 e um máximo de 10 caracteres."
Aqui já aprece um requisito mais interessante, 

com podemos ver no exemplo a URL encurtada possui um 'path param' com um código, esse código serve para recuperar a url original no banco de dados.

o requisito que o desafio impõe é que esse código tenha um mínimo de 05 e um máximo de 10 caracteres. 

no próximo requisito 
"Apenas letras e números são permitidos no encurtamento."

ele impõe também que esse código possua apenas letras e e números, ou seja, caracteres especiais como (#, $, %) não são permitidos.

o quarto requisito, diz o seguinte:
"A URL encurtada será salva no banco de dados com um prazo de validade (você pode escolher a duração desejada)."

O que ele está pedindo aq é que a url tenha um tempo de vida predeterminado, e quando esse tempo passar, a url deixe de existir no banco. 

E no ultimo requisito,

Que é core, do desafio, e fala da rota de redirecionamento, então:

"Ao receber uma chamada para a URL encurtada `https://xxx.com/DXB6V`, você deve fazer o redirecionamento para a URL original salva no banco de dados. 

"Caso a URL não seja encontrada no banco,"
ou seja, caso ela não exista, ou caso o tempo de vida tenha expirado.

" retorne o código de status `HTTP 404 (Not Found)`."

Por fim temos essa seção de "soluções" onde vc pode encontrar soluções feitas por outros membros da comunidade. 

Caso você tenha interesse de ver outras soluções em outras linguagens, ou até mesmo quiser ler o desafio com mais calma, vou deixar o link do desafio na descrição do vídeo.

### Iniciando o Projeto

Bem, entendido o desafio vamos começar o projeto.

Mas antes de por a mão no código, eu queria explicar mais visualmente como um encurtador de URLs funciona.

Então eu criei esse diagrama no tldraw que mostra como os encurtadores de URLs funcionan.

(Criar o diagrama.)














