## Assinatura do Endpoint

GET - interactiveGroups/{id}/interactives/current/{value}

## Descrição do negócio
Endpoint busca a interativa acontecendo na data especificada no parametro "value".
Também deverá ser enviado o tempo restante, em segundos, caso alguma interativa esteja acontecendo.

## Parametros na URL
id - identificador do grupo de interativa
value - data atual no formato "yyyymmddHHmmss"

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": {
    "interactive": {
      "id": "00000000-0000-0000-0000-000000000000",
      "question": "string",
      "startDate": "2018-11-19T13:01:25.456Z",
      "endDate": "2018-11-19T13:01:25.456Z",
      "remainingTime": 45,
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
}
```