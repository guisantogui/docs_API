## Assinatura do Endpoint

GET - papers/{id}/sets/{setId}

## Descrição do negócio
Endpoint responsável por listar as perguntas de determinado Set

## Parametros na URL
id - identificador do paper
setId - identificador do Set

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

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