## Assinatura do Endpoint

POST - cms/event/

## Descrição do negócio
Endpoint deve persistir um novo objeto e seus vínculos no banco de dados, e deve dar o retorno apenas, quando o objeto estiver persistido.
O endpoint passará a permitir que o usuário vincule o evento em mais de um whitelabel, sendo assim, caso o usuário vincule ou desvincule um whitelabel, os vinculos deverão ser gerenciados.

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
    "id": null,
    "titlePT": "Makadu",
    "titleEN": "Makadu",
    "titleES": "Makadu",
    "acronym": "",
    "descriptionPT": "Description",
    "descriptionEN": "Description",
    "descriptionES": "Description",
    "startDate": "20190205100000", // No formato: yyyyMMddHHmmss
    "endDate": "20190205100000", // No formato: yyyyMMddHHmmss
    "timelineType": "55645645-6545316-0545460-545612",
    "active": true,
    "institutionId": "55645645-6545316-0545460-545612",
    "whiteLabelIds": ["55645645-6545316-0545460-545612", "55645645-6545316-0545460-545612", "55645645-6545316-0545460-545612"],
    "subscribeUrl": "http://goog.gl/subs",
    "supportEmailAddress": "sup@gmail.com"
    "password": "554488",
    "isAnyoneEvaluator": true, 
    //Campos novos
    "order": 5, // Não nulo, default 0
    "placePT": "", // Não nulo, default string.empty
    "placeEN": "", // Não nulo, default string.empty
    "placeES": "", // Não nulo, default string.empty
    "participantsExpectedCount": 457, // Não nulo, default 0
    "categoryPT" : "", // Não nulo, default string.empty
    "categoryEN" : "", // Não nulo, default string.empty
    "categoryES" : "", // Não nulo, default string.empty
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