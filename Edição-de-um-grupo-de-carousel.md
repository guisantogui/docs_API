## Assinatura do Endpoint
PUT - cms/carouselGroup

## Descrição do negócio
Endpoint deve persistir as alterações do objeto e seus vínculos no banco de dados, e deve dar o retorno apenas, quando o objeto estiver persistido.

## Parametros na URL
Não se aplica

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)


##Objeto de envio
```
{
  "id": "8789789789789-9789789-546484-8498",
  "description": "",
  "startDate": "13/12/2019 20:00:08",
  "endDate": "14/12/2019 20:00:08",
  "cycleTime": 45,
  "eventId": "8789789789789-9789789-546484-8498",
  "carouselItems": ["8789789789789-9789789-546484-8498", "8789789789789-9789789-546484-8498", "8789789789789-9789789-546484-8498"]
}
  
```

##Objeto de retorno

```
{
   "response": true
}
```