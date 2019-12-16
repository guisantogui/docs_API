## Assinatura do Endpoint

GET - posts/{id}/comments

## Descrição do negócio
Listagem dos comentários de uma postagem

## Parametros na URL
id - Identificador da postagem

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
      "dateCreated": "2018-11-19T13:01:25.529Z",
      "userNamePosted": "string",
      "userPicture": "string",
      "liked": true,
      "likeCount": 0
    }
  ]
}
```