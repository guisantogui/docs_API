## Assinatura do Endpoint

POST - papers/{id}/sets/{setId}/rating

## Descrição do negócio
Endpoint responsável por enviar as respostas de um set e no seu retorno, trazer as perguntas do próximo

## Parametros na URL
id - identificador do paper
setId - Identificador do set

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
```
[
  {
    "commentary": "string",
    "rating": 0,
    "ratingSetQuestionId": "00000000-0000-0000-0000-000000000000",
    "ratingSetQuestionChoiceId": "00000000-0000-0000-0000-000000000000"
  }
]
```

##Objeto de retorno

```
{
  "response": {
    "id": "00000000-0000-0000-0000-000000000000",
    "isLast": true,
    "questions": [
      {
        "id": "00000000-0000-0000-0000-000000000000",
        "question": "string",
        "questionTypeId": "00000000-0000-0000-0000-000000000000",
        "order": 0,
        "questionChoices": [
          {
            "id": "00000000-0000-0000-0000-000000000000",
            "description": "string",
            "order": 0,
            "isRight": true
          }
        ],
        "answer": {
          "commentary": "string",
          "rating": 0,
          "ratingSetQuestionId": "00000000-0000-0000-0000-000000000000",
          "ratingSetQuestionChoiceId": "00000000-0000-0000-0000-000000000000"
        }
      }
    ],
    "keepGoing": true
  }
}
```