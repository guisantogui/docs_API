## Assinatura do Endpoint

GET - cms/sponsors/{id}

## Descrição do negócio
Endpoint deve trazer as informações do sponsor, bem como seus vinculos com eventos e entidades.

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
Não há

##Objeto de retorno

```
{
  "id": "485129485612394856-641523498615-458613",
  "name": "Patrocinador",
  "presentationPT": "",
  "presentationES": "",
  "presentationEN": "",
  "facebookLink": "",
  "linkedinLink": "",
  "twitterLink": "",
  "instagramkLink": "",
  "genericLink": "",
  "thumbnailImageLink": "http://goog.gl/pn2.png",
  "mainImageLink": "http://goog.gl/pn.png",
  "order": 2,
  "events": [
    {
      "id":"855852489648-5548858555-98988999",
      "title": "titulo do evento",
      "sponsorLevel": "Prata"
    }
    , {
      "id":"855852489648-5548858555-98988999",
      "title": "titulo do evento",
      "sponsorLevel": "Prata"
    }],
  "institutions": [{
      "id":"855852489648-5548858555-98988999",
      "title": "nome da entidade",
      "sponsorLevel": "Prata"
    },
    {
      "id":"855852489648-5548858555-98988999",
      "title": "nome da entidade",
      "sponsorLevel": "Prata"
    }]
}
```