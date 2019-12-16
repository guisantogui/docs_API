## Assinatura do Endpoint

GET - cms/papers/{id}

## Descrição do negócio
Endpoint responsável por buscar os detalhes de um paper.

## Parametros na URL
- id - Identificador do id do paper

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": {
    "id": "000987890=937895-486384-8737383",
    "titlePT": "titulo da langauge",
    "titleEN": "titulo da langauge",
    "titleES": "titulo da langauge",
    "abstractPT": "abstract da langauge",
    "abstractEN": "abstract da langauge",
    "abstractES": "abstract da langauge",
    "categoryPT": "category da langauge",
    "categoryEN": "category da langauge",
    "categoryES": "category da langauge",
    "presentationPlacePT": "place da langauge",
    "presentationPlaceEN": "place da langauge",
    "presentationPlaceES": "place da langauge",
    "uniqueId": "98-09",
    "institutionName": "nome",
    "subjectPT": "",
    "subjectEN": "",
    "subjectES": "",
    "presentationStartDate": "13/10/2019 19:00:00",
    "presentationEndDate": "13/10/2019 19:00:00",
    "mainAuthor": "Nome do autor principal",
    "event": {
        "id": "000987890=937895-486384-8737383",
         "title":"title PT"
    },
    "sets": [
      {
        "id":"000987890=937895-486384-8737383",
        "description": "descriçao"
      },
      {
        "id":"000987890=937895-486384-8737383",
        "description": "descriçao"
      }
    ],
    "posterImage": "http://image.com/png.png"
  }
}
```