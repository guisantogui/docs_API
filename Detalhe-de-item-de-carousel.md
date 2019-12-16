## Assinatura do Endpoint

GET - cms/carousel/{id}

## Descrição do negócio
Endpoint deve trazer as informações do item de carousel, bem como os eventos que está vinculado.
Deverá trazer ainda as especialidades que está vinculado, speaker, talk, grupo de interativa, sponsor ou link da mídia, caso a mídia tenha filhos trazer apenas o link da mídia pai.

## Parametros na URL
id - identificador do item de carousel

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
não há

##Objeto de retorno

```
{
  "response": {
    "id": "8789789789789-9789789-546484-8498",
    "description": "",
    "startDate": "13/12/2019 20:00:08",
    "endDate": "14/12/2019 20:00:08",
    "order": null,
    "externalLink": "http://makadu.net",
    "events": [
      {
        "id": "8789789789789-9789789-546484-8498",
        "title": "SOCERGS"
      },
      {
        "id": "8789789789789-9789789-546484-8498",
        "title": "SBC"
      }
    ],
//NOVO
    "mediaLink": "http://Media.com/media.pdf",
    "thumbnailLink": "http://Media.com/thumbail.jpg",
    "institutions": [
      {
        "id": "8789789789789-9789789-546484-8498",
        "title": "SBACV"
      },
      {
        "id": "8789789789789-9789789-546484-8498",
        "title": "Makadu"
      }
    ],
    "speaker": { //null
      "id": "8789789789789-9789789-546484-8498",
      "name": "João"
    },
    "interactiveGroup": {//null
      "id": "8789789789789-9789789-546484-8498",
      "name": "Grupo de Interativa"
    },
    "talk": {//null
      "id": "8789789789789-9789789-546484-8498",
      "name": "Grupo"
    },
    "sponsor": {//null
      "id": "8789789789789-9789789-546484-8498",
      "name": "Patrocinador"
    }
  }
}
```