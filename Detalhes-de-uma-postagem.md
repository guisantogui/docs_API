## Assinatura do Endpoint

GET - posts/{id}

## Descrição do negócio
Retorna informações da postagem e seus comentários.

## Parametros na URL
id - Identificador da postagem

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": {
    "comments": [
      {
        "id": "00000000-0000-0000-0000-000000000000",
        "text": "string",
        "userId": "string",
        "dateCreated": "2018-11-19T13:01:25.604Z",
        "userNamePosted": "string",
        "userPicture": "string",
        "liked": true,
        "likeCount": 0
      }
    ],
    "userVerified": true,
    "postType": 1,
    "medias": [
      {
        "dateCreated": "2018-11-19T13:01:25.604Z",
        "videoLength": "string",
        "mediaType": {
          "id": "00000000-0000-0000-0000-000000000000",
          "name": "string"
        },
        "id": "00000000-0000-0000-0000-000000000000",
        "description": "string",
        "url": "string",
        "mediaTypeId": "00000000-0000-0000-0000-000000000000",
        "order": 0
      }
    ],
    "dateToUnpin": "2018-11-19T13:01:25.604Z",
    "featuredColor": "string",
    "id": "00000000-0000-0000-0000-000000000000",
    "text": "string",
    "userId": "string",
    "datePosted": "2018-11-19T13:01:25.604Z",
    "userNamePosted": "string",
    "userPicture": "string",
    "liked": true,
    "likeCount": 0,
    "commentCount": 0
  }
}
```