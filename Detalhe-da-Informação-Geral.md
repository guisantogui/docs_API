## Assinatura do Endpoint

GET - cms/generalInfos/{id}

## Descrição do negócio
Endpoint deve trazer as informações da informação geral, bem como seus vínculos com eventos e entidades.

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
Não há

##Objeto de retorno

```
{
  "title": "generalInfo",
  "description": "Informação Geral",
  "type": {
    "id": "855852489648-5548858555-98988999",
    "name": "titulo do evento"
  },
  "formatAsHtml": true,
  "order": 2,
  "active": true,
  "image": "http://google.com/img.png",
  "events": [
    {
      "id":"855852489648-5548858555-98988999",
      "title": "titulo do evento"
      }
    , {
      "id":"855852489648-5548858555-98988999",
      "title": "titulo do evento"
    }],
  "institutions": [{
      "id":"855852489648-5548858555-98988999",
      "title": "nome da entidade"
      },
    {
      "id":"855852489648-5548858555-98988999",
      "title": "nome da entidade"
    }]
}
```