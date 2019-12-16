## Assinatura do Endpoint

POST - cms/interactiveGroups/

## Descrição do negócio
Endpoint que cria uma nova entidade, e retorna se a criação foi feita com sucesso.

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
```
{
  "id": null,
  "name": "grupo interativa",
  "labelDate": "Dia 10",
  "place": "sala 05",
  "eventId": "444444444-888888888-9999999",
  "carouselId": "444444444-888888888-9999999",
  "active": true,
  "interactives": [
    "444444444-888888888-9999999",
    "444444444-888888888-9999999",
    "444444444-888888888-9999999"
    ]
}
```

##Objeto de retorno

```
{
  "response": true
}
```