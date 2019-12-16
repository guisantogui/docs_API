## Assinatura do Endpoint

PUT - cms/interactiveGroups/

## Descrição do negócio
Endpoint deve persistir as alterações no objeto e seus vínculos no banco de dados, e deve dar o retorno apenas quando o objeto estiver persistido.

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
```
{
  "id": "444444444-888888888-9999999",
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