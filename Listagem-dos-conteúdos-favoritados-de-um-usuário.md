## Assinatura do Endpoint
GET - users/{id}/contents

## Descrição do negócio
Listagem dos conteúdos favoritados pelo usuário

## Parametros na URL
id - Identificador do usuário

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": [
    {
      "mediaType": "string",
      "id": "00000000-0000-0000-0000-000000000000",
      "medias": [
        {
          "id": "00000000-0000-0000-0000-000000000000",
          "description": "string",
          "url": "string",
          "thumbnailUrl": "string",
          "dateCreated": "2018-11-19T13:01:25.753Z",
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
      ]
    }
  ]
}
```