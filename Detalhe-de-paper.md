## Assinatura do Endpoin
GET - events/{id}/papers/{paperId}

## Descrição do negócio
Exibição dos detalhes de um paper

## Parametros na URL
id - identificador do evento
paperId - identificador do paper

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": {
    "firstSetId": "00000000-0000-0000-0000-000000000000",
    "paperValuation": 0,
    "showPaperEvaluation": true,
    "contents": [
      {
        "id": "00000000-0000-0000-0000-000000000000",
        "description": "string",
        "url": "string",
        "thumbnailUrl": "string",
        "dateCreated": "2018-11-19T13:01:25.226Z",
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
    "eventId": "00000000-0000-0000-0000-000000000000",
    "author": {
      "id": "00000000-0000-0000-0000-000000000000",
      "name": "string"
    },
    "institution": {
      "id": "00000000-0000-0000-0000-000000000000",
      "name": "string"
    },
    "presenter": {
      "id": "00000000-0000-0000-0000-000000000000",
      "name": "string"
    },
    "authors": [
      {
        "id": "00000000-0000-0000-0000-000000000000",
        "name": "string"
      }
    ],
    "evaluator": true,
    "favorited": true,
    "evaluated": true,
    "id": "00000000-0000-0000-0000-000000000000",
    "title": "string",
    "abstract": "string",
    "uniqueId": "string",
    "presentationDateStart": "2018-11-19T13:01:25.226Z",
    "presentationDateEnd": "2018-11-19T13:01:25.226Z",
    "category": "string",
    "presentationPlace": "string",
    "podiumOrder": 0
  }
}
```