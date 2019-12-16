## Assinatura do Endpoint

GET - cms/events/

## Descrição do negócio
Endpoint lista todas eventos do backend, respeitando os filtros e ordenado por:
1. order
2. startDate
3. acronym

## Parametros na URL

####Parametros em via query
- title (somente pesquisar em titulos PT)
- acronym
- active - somente aparecerá entidades ativos, ou inativos, nunca ambos
- category (somente pesquisar em titulos PT)
- supportEmailAddress
- userId
- speakerId
- whiteLabelId
- timelineTypeId
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