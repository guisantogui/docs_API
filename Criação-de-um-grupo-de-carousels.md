## Assinatura do Endpoint
POST - cms/carouselGroup

## Descrição do negócio
Cria um novo grupo de carousel carousel

## Parametros na URL
Não se aplica

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)


##Objeto de envio
```
{
  "description": "",
  "startDate": "20191213200008",
  "endDate": "20191214200008",
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