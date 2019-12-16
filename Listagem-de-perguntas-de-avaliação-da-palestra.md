## Assinatura do Endpoint

GET - cms/talkRatingQuestion/

## Descrição do negócio
Endpoint lista todas eventos do backend, respeitando os filtros e ordenado por:
1. event
2. question

## Parametros na URL

####Parametros em via query
- question - texto da pergunta
- event - pesquisar na propriedade title (em PT), fazendo join pelas talks
- talk -  pesquisar na propriedade title (em PT)
- [Parâmetros de paginação](/API-\(Endpoints\)/Parâmetros-de-paginação)


##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": [
    {
      "id": "988794564896-4856489-55120",
      "question": "",
      "talk: "" //titulo da propriedade talk
    },
    {
      "id": "988794564896-4856489-55120",
      "question": "",
      "talk: "" //titulo da propriedade talk
    },
  ]
}
```