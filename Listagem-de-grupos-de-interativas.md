## Assinatura do Endpoint
GET - events/{id}/interactiveGroups

## Descrição do negócio
Listagem de grupos de interativas, apenas os grupos ativos são listados. Caso exista alguma pergunta acontecendo no momento, a propriedade _answersOptions_ deverá ser preenchida.
Também deverá ser enviado o tempo restante, em segundos, caso alguma interativa esteja acontecendo.
A Busca deixará de buscar informações na talk, o vínculo com a talk não faz mais sentido.

## Parametros na URL
id - Uma breve descrição do parametro

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
      "name": "string",
      "place": "string",
      "startDate": "2018-11-19T13:01:25.347Z",
      "endDate": "2018-11-19T13:01:25.347Z",
      "labelDate": "string",
      "interactive": {
        "id": "00000000-0000-0000-0000-000000000000",
        "question": "string",
        "startDate": "2018-11-19T13:01:25.348Z",
        "endDate": "2018-11-19T13:01:25.348Z",
        "remainingTime": 38,
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
    }
  ]
}
```