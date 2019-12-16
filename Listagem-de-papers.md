## Assinatura do Endpoint

GET - events/{id}/papers

## Descrição do negócio
Listagem dos papers do evento

## Parametros na URL
id - identificador do evento

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": [
    {
      "category": "string",
      "subCategories": [
        {
          "startDate": "2018-11-19T13:01:25.210Z",
          "papers": [
            {
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
              "presentationDateStart": "2018-11-19T13:01:25.210Z",
              "presentationDateEnd": "2018-11-19T13:01:25.210Z",
              "category": "string",
              "presentationPlace": "string",
              "podiumOrder": 0
            }
          ]
        }
      ]
    }
  ]
}
```