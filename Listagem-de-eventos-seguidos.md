## Assinatura do Endpoint

GET - /events/followed

## Descrição do negócio
Lista os eventos que o usuário adicionou aos "Meus eventos"

## Parametros na URL
Não há

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
      "title": "string",
      "startDate": "2018-11-19T13:01:25.154Z",
      "endDate": "2018-11-19T13:01:25.154Z",
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