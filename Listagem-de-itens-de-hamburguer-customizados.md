## Assinatura do Endpoint

GET - cms/hamburguerCustom/

## Descrição do negócio
Endpoint lista todos os itens de hamburguer customizados, ordenado por
1. Evento (title PT)
2. Order

## Parametros na URL

####Parametros em via query

- Id do Evento, filtra equals no Id do evento que poderá estar vinculado
- Title do evento PT, filtra contains no Title (PT) do evento que pdoerá estar vinculado
- Id da Institution, filtra equals no Id da Institution que poderá estar vinculado
- Name da Institution, filtra contains no name da Institution que poderá estar vinculado
- Ativo, sim, não ou ambos
- LabelCustomizado, filtra contains no custom das tabelas HamburguerItemInstitutionLanguage e HamburguerItemEventLanguage
- LabelDefault (id), filtra equals no Id

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
      "baseLabel": "Uma escolha",
      "customLabel": "title do evento PT",
      "order": 8,
      "active": true,
      "event": "Title PT",
      "instituion": "Name"
    },
    {
      "id": "988794564896-4856489-55120",
      "baseLabel": "Uma escolha",
      "customLabel": "title do evento PT",
      "order": 8,
      "active": true,
      "event": "Title PT",
      "instituion": "Name"
    }
  ]
}
```