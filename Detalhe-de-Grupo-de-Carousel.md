## Assinatura do Endpoint
GET - cms/carouselGroup/{id}

## Descrição do negócio
Detalha os itens do grupo decarousel

## Parametros na URL
Não se aplica

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
id - identificador do grupo de carousel

##Objeto de retorno

```
{
  "response": {
    "description": "",
    "startDate": "13/12/2019 20:00:08",
    "endDate": "14/12/2019 20:00:08",
    "cycleTime": 45,
    "eventId": "8789789789789-9789789-546484-8498",
    "carouselItems": [
      {
        "id": "8789789789789-9789789-546484-8498",
        "description": "carousel X"
      },
      {
        "id": "8789789789789-9789789-546484-8498",
        "description": "carousel X"
      }
    ]
  }
}
```