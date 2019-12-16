## Assinatura do Endpoint

GET - cms/eventRatingQuestions/

## Descrição do negócio
Endpoint lista todos as perguntas de avaliação de evento, ordenado por
1. Evento (title PT)
2. Order

## Parametros na URL

####Parametros em via query

- Id do Evento, filtra equals no Id do evento que poderá estar vinculado
- Title do evento PT, filtra contains no Title (PT) do evento que poderá estar vinculado
- Texto da pergunta, filtra contains na Question da eventRatingQuestion

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
      "question": "Question na linguagem PT",
      "order": 8,
      "event": "Title PT"
    },
    {
      "id": "988794564896-4856489-55120",
      "question": "Question PT",
      "order": 9,
      "event": "Title PT"
    }
  ]
}
```