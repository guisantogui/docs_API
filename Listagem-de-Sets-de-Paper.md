## Assinatura do Endpoint

GET - cms/sets/

## Descrição do negócio
Endpoint lista todos sets de papers do backend, respeitando os filtros e ordenado por:
1. event
2. order DESC

## Parametros na URL

####Parametros em via query
- Description, filtra contais na propriedade description do Set
- Id do Evento, filtra equals no Id do evento que papers poderão estar vinculados
- Title do evento PT, filtra contains no Title (PT) do evento que papers poderão estar vinculados
- Titulo Paper PT, filtra contains no Title (PT) de papers vinculados
- UniqueId Paper, filtra contains no UniqueId de papers vinculados
- HasQuestions, filtra se há perguntas no set, se não há, ou ambos (true, false, não envia)
- HasPaper, filtra se o set está em algum paper, se não há, ou ambos (true, false, não envia)


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
      "description": "",
      "event": "title do evento PT",
      "order": 8,
      "paper": "title do paper PT"
      "hasQuestions": false
    },
    {
      "id": "988794564896-4856489-55120",
      "description": "",
      "event": "title do evento",
      "order": 8,
      "paper": "title do paper PT"
      "hasQuestions": false
    }
  ]
}
```