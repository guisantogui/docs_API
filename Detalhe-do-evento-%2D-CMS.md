## Assinatura do Endpoint

GET - cms/events/{id}

## Descrição do negócio
Endpoint lista todas informações do evento.

## Parametros na URL
id - Identificador do evento

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
    "id": "0050505-080808-845454545-48745154",
    "titlePT": "Makadu",
    "titleEN": "Makadu",
    "titleES": "Makadu",
    "acronym": "",
    "descriptionPT": "Description",
    "descriptionEN": "Description",
    "descriptionES": "Description",
    "startDate": "10/02/2019 10:00:00",
    "endDate": "11/02/2019 10:00:00",
    "timelineType": "55645645-6545316-0545460-545612",
    "active": true,
    "institution": {
        "id": "55645645-6545316-0545460-545612",
        "name": "institution"
     },
    "whiteLabel": [{
        "id": "55645645-6545316-0545460-545612",
        "name": "WL1"
     },
     {
        "id": "55645645-6545316-0545460-545612",
        "name": "WL2"
     },
     {
        "id": "55645645-6545316-0545460-545612",
        "name": "WL3"
     }],
    "subscribeUrl": "http://goog.gl/subs",
    "supportEmailAddress": "sup@gmail.com"
    "password": "554488",
    "isAnyoneEvaluator": true, 
    "order": 5, 
    "placePT": "",
    "placeEN": "",
    "placeES": "", 
    "participantsExpectedCount": 457, 
    "categoryPT" : "", 
    "categoryEN" : "",
    "categoryES" : "",
    "bannerUrlPT" : "", 
    "bannerUrlEN" : "",
    "bannerUrlES" : ""

}
```