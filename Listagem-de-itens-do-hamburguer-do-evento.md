## Assinatura do Endpoint

GET - hamburguers/byEvent/{eventId}

## Descrição do negócio
Lista os itens de menu daquele evento, somente itens ativos são listados, e itens personalizados já trazem seu label especial.

## Parametros na URL
eventId - identificador do evento

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
      "label": "string",
      "order": 0,
      "notificationCount": 0
    }
  ]
}
```