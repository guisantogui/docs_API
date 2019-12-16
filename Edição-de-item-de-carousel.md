## Assinatura do Endpoint
PUT - cms/carousel

## Descrição do negócio
Endpoint deve persistir as alterações do objeto e seus vínculos no banco de dados, e deve dar o retorno apenas, quando o objeto estiver persistido.
Observação, um item de carousel não poderá ter seu tipo alterado, a menos que seja um link simples, ou seja, não tenha especializações, como interativa, palestrante, sponsor, palestra ou mídia.
Caso as flags de remoção venham com valor true, deverá ser removido fisicamente os registros do banco, bem como binários.

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
      "id": "8789789789789-9789789-546484-8498",
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
      "interactiveId": null, //"8789789789789-9789789-546484-8498",
//NOVO
      "institutions": ["8789789789789-9789789-546484-8498", "8789789789789-9789789-546484-8498"],
      "removeMedia": true,
      "removeThumbnail": false
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