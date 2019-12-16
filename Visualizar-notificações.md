## Assinatura do Endpoint

PUT - events/{id}/notifications/seen

## Descrição do negócio
Endpoint que marca como visualizada uma listagem de notificações

## Parametros na URL
id - identificador do evento

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio

```
[
  {
    "id": "00000000-0000-0000-0000-000000000000",
    "dateSeen": "string",
    "notificationType": 1
  }
]
```

##Objeto de retorno

```
{
  "response": true
}
```