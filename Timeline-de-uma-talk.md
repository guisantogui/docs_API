## Assinatura do Endpoint

GET - talks/{id}/posts
## Descrição do negócio
O endpoint deverá listar as postagens daquele paper, ordenado pelos seguinte critérios
1º - Maior quantidade de curtidas
2º - Postagem mais nova

A busca das postagens passará a ser paginada.

## Parametros na URL
id - Identificador da talk

###Parametros query
skip - valor inteiro que define o post atual para paginação, assim pulando a quantidade definida na hora de buscar na base de dados
take - valor inteiro que define a quantidade de posts buscados a cada paginação

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

Esse endpoint deverá ser versionado para a versão 2 então o header que manda a versão deverá passar a enviar a versão 2, a versão 1 deverá continuar funcionando.

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": [
    {
      "id": "00000000-0000-0000-0000-000000000000",
      "text": "string",
      "userId": "string",
      "datePosted": "2018-11-19T13:01:25.655Z",
      "userNamePosted": "string",
      "userPicture": "string",
      "liked": true,
      "likeCount": 0,
      "commentCount": 0
    }
  ]
}
```