## Assinatura do Endpoint
GET - /institutions/{id}/events

## Descrição do negócio
Retorna todos eventos ativos vinculados naquela entidade

## Parametros na URL
id - Identificador da Entidade

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não existe

##Objeto de retorno

```
{
  "response": [
    {
      "id": "00000000-0000-0000-0000-000000000000",
      "title": "string",
      "startDate": "2018-11-14T17:10:52.972Z",
      "endDate": "2018-11-14T17:10:52.972Z",
      "institutionId": "00000000-0000-0000-0000-000000000000",
      "description": "string",
      "supportEmailAddress": "string",
      "bannerUrl": "string",
      "showPaperEvaluation": true,
      "isAnyoneEvaluator": true,
      "subscribeUrl": "string",
      "providerSettingId": "00000000-0000-0000-0000-000000000000",
      "active": true,
      "timelineInteractionType": 1,
      "password": "string"
    }
  ]
}
```

