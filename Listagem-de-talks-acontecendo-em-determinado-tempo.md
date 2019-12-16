
## Assinatura do Endpoint

GET - events/{id}/talks/time/{value}

## Descrição do negócio
Listagem das palestras que acontecerão nos 15 minutos seguintes ao valor enviado por parâmetro _value_

## Parametros na URL
id - Identificador do evento
value - data parametro para pegar as palestras nos 15 minutos subsequentes, sempre enviada no formato "yyyyMMddhhmmss"

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": [
    {
      "favorited": true,
      "id": "00000000-0000-0000-0000-000000000000",
      "title": "string",
      "description": "string",
      "startDate": "2018-11-19T13:01:25.305Z",
      "endDate": "2018-11-19T13:01:25.305Z",
      "room": "string",
      "category": "string",
      "featuredColor": "string"
    }
  ]
}
```
