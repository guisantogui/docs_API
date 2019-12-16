## Assinatura do Endpoint

POST - talks/{id}/ratings/answers

## Descrição do negócio
Avaliação complexa, com respostas para todas perguntas de cada palestra.

## Parametros na URL
id - Identificador da palestra 

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
```
{
  "comment": "string",
  "questions": [
    {
      "questionId": "00000000-0000-0000-0000-000000000000",
      "rating": 0
    }
  ]
}
```

##Objeto de retorno

```
{
  "response": true
}
```