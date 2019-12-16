## Assinatura do Endpoint

PUT - cms/event/

## Descrição do negócio
Endpoint deve persistir as alterações no objeto e seus vínculos no banco de dados, e deve dar o retorno apenas quando o objeto estiver persistido.
O endpoint passará a permitir que o usuário vincule / desvincule o evento em mais de um whitelabel, sendo assim, caso o usuário vincule ou desvincule um whitelabel, os vinculos deverão ser gerenciados.

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

Até 3 arquivos binários (Imagem da postagem, enviado como Multipart header)
- BannerPT
- BannerES
- BannerEN

Json: Texto da postagem, enviada string com encoding = "x-www-form-urlencoded" no formato json abaixo:

```
{
    "id": "D6B42953-944D-4DC7-89DC-3070AE7D4371",
    "titlePT": "CardioPed",
    "titleEN": "",
    "titleES": "",
    "acronym": "CARDIO",
    "descriptionPT": "CARDIO",
    "descriptionEN": "",
    "descriptionES": "",
    "startDate": "20190205100000",
    "endDate": "20190205100000",
    "timelineType": 1,
    "active": true,
    "institutionId": null,
    "whiteLabelId": ["B5576F8B-699C-4EB1-9955-3120EA25113A", "B5576F8B-699C-4EB1-9955-3120EA25113A", "B5576F8B-699C-4EB1-9955-3120EA25113A"],
    "subscribeUrl": "http://goog.gl/subs",
    "supportEmailAddress": "sup@gmail.com",
    "password": "",
    "isAnyoneEvaluator": false, 
    "order": 5,
    "placePT": "",
    "placeEN": "",
    "placeES": "",
    "participantsExpectedCount": 457,
    "categoryPT" : "",
    "categoryEN" : "",
    "categoryES" : "",    
    "removeBannerUrlPT": false,
    "removeBannerUrlEN": false,
    "removeBannerUrlES": false
}
```

##Objeto de envio
Não há

##Objeto de retorno

```
{
  "response": true
}
```