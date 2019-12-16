## Assinatura do Endpoint
GET - /events/byWhiteLabel

## Descrição do negócio
Retorna todos eventos ativos vinculados naquele white label.
A propriedade ```accreditationContent``` deverá ser retornada com base na seguinte regra:
 - Caso o evento não esteja presente na tabela SubscriptionIntegration, deverá retornar string vazia
 - Caso o usuário que fez o request não tenha seu email na tabela (comparando com emails com ```.trim()```), deverá retornar string vazia
 - Caso o evento esteja na tabela, porém o email do usuário não esteja presente para aquele evento, deverá retornar string vazia
 - Caso o email do usuário esteja presente, porém o evento não esteja presente na tabela, deverá retornar string vazia
 - Caso o email do usuário esteja presente, e relacionado com o evento, deverá retornar, o ```externalId``` relacionado com a propriedade ```AccreditationDefaultContent```.

####Regra de relacionamento entre ```externalId``` e ```AccreditationDefaultContent``` 
 - Caso ```AccreditationDefaultContent``` seja NULL, deverá retornar apenas o valor de ```externalId```
 - Caso ```AccreditationDefaultContent``` não seja null, deverá tentar concatenar o valor na posição 0, exemplo:
texto_ac_{0}_continua_texto


## Parametros na URL
Sem parâmetros

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
      "accreditationContent": "codigo_de_credenciamento"
    }
  ]
}
```

