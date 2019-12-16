## Assinatura do Endpoint

GET - speakers/{id}

## Descrição do negócio
Endpoint responsável por buscar as informações do palestrante, bem como suas palestras, sendo que as palestras devem ter a informação de qual evento pertencem.
Esse endpoint deverá ser versionado para versão de número 2, para manter compatibilidade com aplicativos antigos.

## Parametros na URL
id - Identificador do palestrante

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": {
    "events": [
      {
        "id": "00000000-0000-0000-0000-000000000000",
        "title": "Titulo de acrodo com a tabela de linguagem",
        "talks": [
          {
            "favorited": true,
            "id": "00000000-0000-0000-0000-000000000000",
            "title": "string",
            "description": "string",
            "startDate": "2018-11-19T13:01:25.618Z",
            "endDate": "2018-11-19T13:01:25.618Z",
            "room": "string",
            "category": "string",
            "featuredColor": "string"
          }, 
          {
            "favorited": true,
            "id": "00000000-0000-0000-0000-000000000000",
            "title": "string",
            "description": "string",
            "startDate": "2018-11-19T13:01:25.618Z",
            "endDate": "2018-11-19T13:01:25.618Z",
            "room": "string",
            "category": "string",
            "featuredColor": "string"
          }
        ]
      },
      {
        "id": "00000000-0000-0000-0000-000000000000",
        "title": "Evento 2",
        "talks": [
          {
            "favorited": true,
            "id": "00000000-0000-0000-0000-000000000000",
            "title": "string",
            "description": "string",
            "startDate": "2018-11-19T13:01:25.618Z",
            "endDate": "2018-11-19T13:01:25.618Z",
            "room": "string",
            "category": "string",
            "featuredColor": "string"
          }, 
          {
            "favorited": true,
            "id": "00000000-0000-0000-0000-000000000000",
            "title": "string",
            "description": "string",
            "startDate": "2018-11-19T13:01:25.618Z",
            "endDate": "2018-11-19T13:01:25.618Z",
            "room": "string",
            "category": "string",
            "featuredColor": "string"
          }
        ]
      }
    ],
    "about": "string",
    "cpf": "string",
    "email": "string",
    "profilePictureUrl": "string",
    "id": "00000000-0000-0000-0000-000000000000",
    "name": "string"
  }
}
```