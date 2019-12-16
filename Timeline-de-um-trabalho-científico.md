## Assinatura do Endpoint

GET - papers/{id}/posts

## Descrição do negócio
Listagem dos posts da timeline de um trabalho científico

## Parametros na URL
id - Identificador do trabalho científico

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

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
      "datePosted": "2018-11-19T13:01:25.507Z",
      "userNamePosted": "string",
      "userPicture": "string",
      "liked": true,
      "likeCount": 0,
      "commentCount": 0
    }
  ]
}
```