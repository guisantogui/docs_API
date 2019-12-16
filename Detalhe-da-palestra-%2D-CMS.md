## Assinatura do Endpoint

GET - cms/talks/{id}

## Descrição do negócio
Endpoint que busca todas informações pertinentes a talk

## Parametros na URL
id - Identificador da talk

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": {
    "id": "00000000-0000-0000-0000-000000000000",
    "titlePT": "string",
    "titleEN": "string",
    "titleES": "string",
    "descriptionPT": "string",
    "descriptionEN": "string",
    "descriptionES": "string",
    "startDate": "2018-11-19T13:01:25.704Z",
    "endDate": "2018-11-19T13:01:25.704Z",
    "roomPT": "string",
    "roomEN": "string",
    "roomES": "string",
    "categoryPT": "string",
    "categoryEN": "string",
    "categoryES": "string",
    "featuredColor": "string",
    "autolike": true,
    "active": true,
    "event": {
      "id": "00000000-0000-0000-0000-000000000000",
      "name": "Evento 2"
    },
    "carousels": [{
      "id": "00000000-0000-0000-0000-000000000000",
      "name": "Evento 2"
    },
    {
      "id": "00000000-0000-0000-0000-000000000000",
      "name": "Evento 2"
    },
    "speakers": [{
      "id": "00000000-0000-0000-0000-000000000000",
      "name": "João"
    },
    {
      "id": "00000000-0000-0000-0000-000000000000",
      "name": "Carlos"
    }]
  }
}
```