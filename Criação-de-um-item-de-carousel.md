## Assinatura do Endpoint
POST - cms/carousel

## Descrição do negócio
Cria um novo carousel

## Parametros na URL
Não se aplica

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

Até 2 arquivos binários (Imagem da postagem, enviado como Multipart header)
- thumbnail
- media

Json: Texto da postagem, enviada string com encoding = "x-www-form-urlencoded" no formato json abaixo:
```
{
      "description": "",
      "startDate":"13/12/2019 20:00:08",
      "endDate":"14/12/2019 20:00:08",
      "order": null,
      "externalLink":"http://makadu.net",
      "events": ["8789789789789-9789789-546484-8498",
      "8789789789789-9789789-546484-8498", "8789789789789-9789789-546484-8498"],
      "sponsorId": null, //"8789789789789-9789789-546484-8498"
      "speakerId": null, //"8789789789789-9789789-546484-8498"
      "talkId": null, //"8789789789789-9789789-546484-8498"
      "interactiveId": null, //"8789789789789-9789789-546484-8498"
//NOVO
      "institutions": ["8789789789789-9789789-546484-8498",
      "8789789789789-9789789-546484-8498", "8789789789789-9789789-546484-8498"],
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