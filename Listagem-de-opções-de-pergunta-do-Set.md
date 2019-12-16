## Assinatura do Endpoint

GET - cms/setQuestionChoices/

## Descrição do negócio
Endpoint lista todas as opções de perguntas de sets dos papers, ordenado por
1. Evento (title PT)

## Parametros na URL

####Parametros em via query

- Opção, filtra contains na propriedade ChoiceText do RatingSetQuestionChoice
- Id do Evento, filtra equals no Id do evento que papers poderão estar vinculados
- Title do evento PT, filtra contains no Title (PT) do evento que papers poderão estar vinculados
- Id do Set, filtra equals no Id do set que pode estar vinculado
- Description do Set, filtra contains na Description do set que poderá estar vinculados
- Id da Pergunta, filtra equals no Id da pergunta que pode estar vinculada
- Question do Pergunta, filtra contains na Question da pergunta que poderá estar vinculada
- HasQuestion, filtra se a Choice está em alguma pergunta, se não há, ou ambos (true, false, não envia)


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
      "choice": "Uma escolha",
      "event": "title do evento PT",
      "order": 8,
      "question": "pergunta vinculada",
      "set": "Set vinculado à pergunta vinculada",
      "isRight": true
    },
    {
      "id": "988794564896-4856489-55120",
      "choice": "Uma escolha",
      "event": "title do evento PT",
      "order": 8,
      "question": "pergunta vinculada",
      "set": "Set vinculado à pergunta vinculada",
      "isRight": true
    }
  ]
}
```