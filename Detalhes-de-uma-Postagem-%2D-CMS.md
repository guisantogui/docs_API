## Assinatura do Endpoint

GET - cms/posts/{id}

## Descrição do negócio
Endpoint deve retornar o objeto referente ao Id enviado por parâmetro

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
Não há

##Objeto de retorno

```
{
    "id": "78787878-99999-51545454-222111-6622411",
    "text": "Makadu",
    "userdId": { 
      "id": "55558888945",
      "name": "joão"
    },
    "event": {
        "id": "78787878-99999-51545454-222111-6622411",
        "title": "SOCERGS" <-- Pegar a propriedade na lingua portuguesa
     },
    "institution": null, <-- propriedades id (GUID) e name (String)
    "pinDate": "11/12/2019 12:15:15",
    "unPinDate": "11/12/2019 12:15:15",
    "featuredColor": "#885544",
    "postDate": "11/12/2019 11:15:15",
    "active": true, 
    "postPicture": "http://www.imagem.com/image.png"

}
```