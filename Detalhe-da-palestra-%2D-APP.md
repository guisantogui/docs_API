## Assinatura do Endpoint

GET - talks/{id}

## Descrição do negócio
Endpoint que busca todas informações pertinentes a talk

## Parametros na URL
id - Identificador da talk

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": {
    "rating": {
      "rating": 0,
      "comment": "string"
    },
    "questions": [
      {
        "rating": 0,
        "questionId": "00000000-0000-0000-0000-000000000000",
        "questionDescription": "string"
      }
    ],
    "contents": [
      {
        "id": "00000000-0000-0000-0000-000000000000",
        "description": "string",
        "url": "string",
        "thumbnailUrl": "string",
        "dateCreated": "2018-11-19T13:01:25.702Z",
        "videoLength": "string",
        "mediaType": {
          "id": "00000000-0000-0000-0000-000000000000",
          "name": "string"
        },
        "featured": true,
        "order": 0,
        "speaker": {
          "id": "00000000-0000-0000-0000-000000000000",
          "name": "string"
        },
        "children": [
          {}
        ],
        "favorited": true
      }
    ],
    "generalInfos": [
      {
        "id": "00000000-0000-0000-0000-000000000000",
        "description": "string",
        "title": "string",
        "formatDescriptionAsHtml": true,
        "imageUrl": "string",
        "order": 0,
        "generalInfoTypeId": "00000000-0000-0000-0000-000000000000"
      }
    ],
    "speakers": [
      {
        "about": "string",
        "cpf": "string",
        "email": "string",
        "profilePictureUrl": "string",
        "id": "00000000-0000-0000-0000-000000000000",
        "name": "string"
      }
    ],
    "id": "00000000-0000-0000-0000-000000000000",
    "title": "string",
    "description": "string",
    "startDate": "2018-11-19T13:01:25.704Z",
    "endDate": "2018-11-19T13:01:25.704Z",
    "room": "string",
    "category": "string",
    "featuredColor": "string"
  }
}
```