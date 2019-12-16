
## Assinatura do Endpoint

GET - institutions/{id}/carousels

## Descrição do negócio
Endpoint que lista os itens de carousel que são exibidos acima da timeline da entidade, que são dos possíveis tipos:
- Palestra
- Palestrante
- Patrocinador
- Conteúdo
- Interativa
- Link Simples
- Sem link

## Parametros na URL
id - Identificador da entidade

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
      "thumbnail": "string",
      "externalLink": "string",
      "exclude": true,
      "medias": [
        {
          "id": "00000000-0000-0000-0000-000000000000",
          "description": "string",
          "url": "string",
          "thumbnailUrl": "string",
          "dateCreated": "2018-11-19T13:01:25.286Z",
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
      "talk": {
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
        "startDate": "2018-11-19T13:01:25.286Z",
        "endDate": "2018-11-19T13:01:25.286Z",
        "room": "string",
        "category": "string",
        "featuredColor": "string"
      },
      "interactiveGroup": {
        "id": "00000000-0000-0000-0000-000000000000",
        "name": "string",
        "place": "string",
        "startDate": "2018-11-19T13:01:25.286Z",
        "endDate": "2018-11-19T13:01:25.286Z",
        "labelDate": "string",
        "interactive": {
          "id": "00000000-0000-0000-0000-000000000000",
          "question": "string",
          "startDate": "2018-11-19T13:01:25.286Z",
          "endDate": "2018-11-19T13:01:25.286Z",
          "order": 0,
          "time": 0,
          "interactiveTypeId": "00000000-0000-0000-0000-000000000000",
          "answersOptions": [
            {
              "id": "00000000-0000-0000-0000-000000000000",
              "order": 0,
              "description": "string",
              "isRight": true
            }
          ]
        }
      },
      "speaker": {
        "id": "00000000-0000-0000-0000-000000000000",
        "name": "string"
      },
      "sponsor": {
        "id": "00000000-0000-0000-0000-000000000000",
        "name": "string"
      }
      "type": 1
    }
  ]
}
```
