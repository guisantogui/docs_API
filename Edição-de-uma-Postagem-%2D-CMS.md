## Assinatura do Endpoint

PUT - cms/posts/

## Descrição do negócio
Endpoint responsável por editar, uma postagem, lembrando que usuários poderão ser revinculados. 
Em caso da timeline ser revinculada, a postagem deverá perder todas curtidas e comentários atrelados.
O parâmetro ```removeImage``` controlará se a imagem atual da postagem deverá ser deletada, se uma nova imagem for enviada deverá atualizar a antiga, ou adicionar a postagem.

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

Até 1 arquivos binários (Imagem da postagem, enviado como Multipart header)
- Image

Json: Texto da postagem, enviada string com encoding = "x-www-form-urlencoded" no formato json abaixo:

```
{
    "id": "78787878-99999-51545454-222111-6622411",
    "text": "Makadu",
    "userdId": "5555-55588-8555-8888945",
    "pinDate": "20191211100908",
    "unPinDate": "20191211100908",
    "featuredColor": "#885544",
    "postDate": "20191211100908", //Schedule
    "eventId": "55555-99988552145-63555455", // nullable
    "institutionId": "55555-99988552145-63555455", // nullable
    "talkId": "55555-99988552145-63555455", // nullable
    "paperId": "55555-99988552145-63555455", // nullable
    "removeImage": true
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