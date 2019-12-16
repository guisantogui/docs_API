## Assinatura do Endpoint

GET - cms/setQuestions/

## Descrição do negócio
Endpoint lista todas as perguntas de sets dos papers, ordenado por
1. Evento (title PT)
2. Order (do objeto ratingSet)

## Parametros na URL

####Parametros em via query
- Pergunta, filtra contais na propriedade question do RatingSetQuestion
- Id do Set, filtra equals no Id do set que pode estar vinculado
- Description do Set, filtra contains na Description do set que poderá estar vinculados
- Type, filtra pelo Id do tipo da pergunta (RatingSetQuestionType), ou não filtra se não for enviado
- Id do Evento, filtra equals no Id do evento que papers poderão estar vinculados
- Title do evento PT, filtra contains no Title (PT) do evento que papers poderão estar vinculados
- HasChoices, filtra se há opções na pergunta, se não há, ou ambos (true, false, não envia) - **OBS: Se esse filtro for enviado, somente perguntas do tipo de múltipla escolha devem retornar**
- hasSet, filtra se a pergunta está em algum set, se não há, ou ambos (true, false, não envia)


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
      "event": "title do evento PT",
      "order": 8,
      "set": "descrição do set",
      "type": "Multipla escolha"
    },
    {
      "id": "988794564896-4856489-55120",
      "question": "",
      "event": "title do evento PT",
      "order": 5,
      "set": "descrição do set",
      "type": "Numérica"
    }
  ]
}
```