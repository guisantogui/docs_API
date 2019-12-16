## Assinatura do Endpoint

POST - cms/posts/

## Descrição do negócio
Endpoint deve persistir um novo objeto e seus vínculos no banco de dados, e deve dar o retorno apenas, quando o objeto estiver persistido.

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

Até 1 arquivos binários (Imagem da postagem, enviado como Multipart header)
- Image

Json: Texto da postagem, enviada string com encoding = "x-www-form-urlencoded" no formato json abaixo:

```
{
    "text": "Makadu",
    "userdId": "5555-55588-8555-8888945",
    "pinDate": "20191211100908", // nullable
    "unPinDate": "20191211100908", // nullable
    "featuredColor": "#885544",
    "postDate": "20191211100908", //Schedule & nullable
    "eventId": "55555-99988552145-63555455", // nullable
    "institutionId": "55555-99988552145-63555455", // nullable
    "talkId": "55555-99988552145-63555455", // nullable
    "paperId": "55555-99988552145-63555455", // nullable
    
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