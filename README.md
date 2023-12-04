# resumoApiREST

## Api REST e RESTful

- APIs REST e RESTful são abordagens para projetar e desenvolver interfaces de programação web que seguem os princípios do estilo arquitetural REST. REST é um conjunto de diretrizes que visa fornecer uma estrutura para a comunicação entre sistemas.
  
### 1. APIs REST

- Baseiam-se em princípios como statelessness (ausência de estado).
- Identificação de recursos (cada recurso é único e acessado por meio de URLs).
- Operações sobre recursos utilizando métodos HTTP.
- Os dados são geralmente representados em formatos como JSON ou XML.

### 2. RESTful

- Além dos princípios REST, uma API RESTful busca ser simples, escalável, e fácil de entender.
- Interface uniforme: a API deve fornecer uma interface consistente e padronizada para acessar e manipular recursos.
- Operações baseadas em recursos: as ações realizadas pela API devem ser orientadas a recursos identificados por URLs únicas.
- São consideradas uma implementação mais completa e rigorosa do modelo REST.
  

## Diferenças entre REST e RESTFul

- Ambos seguem os princípios REST, mas o termo "RESTful" é frequentemente usado para descrever implementações específicas que aderem de forma estrita a esses princípios.
- Assim as principais diferenças entre APIs REST e RESTful está no nível de aderência aos princípios REST. Enquanto as APIs REST seguem os princípios básicos do REST, as APIs RESTful são uma implementação mais completa e estrita desses princípios.
- APIs RESTful aderem a critérios adicionais, como a interface uniforme, clientes sem estado e operações baseadas em recursos.
- Uma API RESTful é, essencialmente, uma implementação de uma API REST que segue as melhores práticas e convenções para melhorar a usabilidade e manutenção.

## HTTP verbs

- Os verbos HTTP, também conhecidos como métodos HTTP, são ações que indicam a intenção do cliente em relação a um recurso específico.
- Esses verbos formam a base do protocolo HTTP e são essenciais para a comunicação entre clientes e servidores web.
- Esses métodos são: GET, POST, PUT, DELETE, PATCH, OPTIONS, HEAD, TRACE, CONNECT.
- É importante destacar os 4 mais básicos e essênciais na construção de um CRUD, são o GET, POST, PUT, DELETE.
- A seguir um resumo sobre suas funções: 
  
- GET: Solicita a recuperação de um recurso. É usado para obter dados de um servidor, e não deve ter efeitos colaterais no estado do servidor.

- POST: Envia dados para serem processados a um recurso específico. É frequentemente utilizado para criar novos recursos no servidor.

- PUT: Atualiza um recurso existente ou cria um recurso se ele não existir. Geralmente, envia o recurso completo com as alterações.

- DELETE: Solicita a remoção de um recurso no servidor. Indica que o cliente deseja excluir o recurso especificado.

- PATCH: Aplica modificações parciais a um recurso. É usado para atualizações parciais em um recurso existente.

- OPTIONS: Retorna os métodos HTTP suportados em um determinado recurso. Pode ser usado para verificar as opções de comunicação com o servidor.

- HEAD: Semelhante ao GET, mas é usado para obter apenas os cabeçalhos do recurso, sem o corpo da resposta. É útil para verificar informações de cabeçalho sem recuperar todo o conteúdo.

- TRACE: Permite ao cliente obter informações de diagnóstico sobre a rota até o recurso de destino. Não é amplamente utilizado devido a questões de segurança.

- CONNECT: O método CONNECT estabelece um túnel para o servidor identificado pelo recurso de destino.


## HTTP Status Code

- Os códigos de status HTTP são retornados pelo servidor para indicar o resultado de uma solicitação feita por um cliente. Eles fornecem informações sobre o sucesso, falha ou outro estado da solicitação.
- O código de status HTTP é uma parte essencial da resposta transmitida do servidor ao cliente. Contudo, você só vai ver quando a comunicação não foi bem sucedida.
- Existem cinco categorias de códigos de status, sendo que o primeiro dígito do código define a classe de resposta. Por exemplo: o código de status 404 pertence à classe 4xx e indica erro no lado do cliente e, o código 502 pertence à classe 5xx e indica erro no lado do servidor.
- São muitos os códigos de status HTTP, divididos entre cliente e servidor, aqui vão alguns exemplos do mais comuns e conhecidos:

### 1. 4xx (Client Error)

- Indica que houve um erro por parte do cliente na solicitação.

- 400 Bad Request: A solicitação do cliente é inválida ou malformada.
- 401 Unauthorized: O cliente deve autenticar para obter acesso.
- 403 Forbidden: O cliente autenticado não tem permissão para acessar o recurso.
- 404 Not Found: O recurso solicitado não foi encontrado no servidor.

### 2. 5xx (Server Error)

- Indica que houve um erro por parte do servidor ao processar a solicitação do cliente.

- 500 Internal Server Error: Um erro genérico interno do servidor.
- 502 Bad Gateway: O servidor, enquanto agindo como gateway ou proxy, recebeu uma resposta inválida do servidor upstream.
- 503 Service Unavailable: O servidor não está pronto para manipular a solicitação. Geralmente, está temporariamente sobrecarregado ou em manutenção.
  

-------------------------------------------------------------------------------------------------------------------------------

 **Autor do resumo: _Eduardo Henrique Bezerra dos Santos_ - 01530700**
