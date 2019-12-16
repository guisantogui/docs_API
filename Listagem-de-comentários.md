## Assinatura do Endpoint

GET - cms/comments/

## Descrição do negócio
Endpoint lista todos comentários do backend, respeitando os filtros e ordenado por:
1. dateCreated DESC

## Parametros na URL

####Parametros em via query
- text (texto do comentário)
- event (somente pesquisar em titulos PT)
- institution (name)
- verifiedUsers (true = sim | false = não | não envia = ambos)
- userEmail (pesquisa pelo email do dono do comentário)
- postText (pelo texto do post a qual o comentário deve pertencer para retornar)
- [Parâmetros de paginação](/API-\(Endpoints\)/Parâmetros-de-paginação)

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": [
    {
      "id": "988794564896-4856489-55120",
      "text": "",
      "userEmail": "",
      "verified": true,
      "postagem": "Texto da postagem a qual pertence",
      "event": "evento A",
      "institution": ""
    },
    {
      "id": "988794564896-4856489-55120",
      "text": "",
      "userEmail": "",
      "verified": true,
      "postagem": "Texto da postagem a qual pertence",
      "event": "",
      "institution": "instituíção B"
    }
  ]
}
```