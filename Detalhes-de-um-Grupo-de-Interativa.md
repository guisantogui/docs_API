## Assinatura do Endpoint

GET - cms/interactiveGroups/{id}

## Descrição do negócio
Endpoint deve trazer as informações do grupo de interativa, bem como suas perguntas

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
Não há

##Objeto de retorno

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
    {
      "id": "444444444-888888888-9999999",
      "name": "Pergunta 2"
    },
    {
      "id": "444444444-888888888-9999999",
      "name": "Pergunta 5"
    },
    {
      "id": "444444444-888888888-9999999",
      "name": "Pergunta 1"
    }
  ]
}
```