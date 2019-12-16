
## Assinatura do Endpoint

GET - events/{id}/rating

## Descrição do negócio
Listagem das perguntas de avaliação do evento, com as respostas do usuário, caso existam

## Parametros na URL
id - identificador do evento

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": [
    {
      "questionId": "00000000-0000-0000-0000-000000000000",
      "questionDescription": "string",
      "textAnswer": "string",
      "rating": 0
    }
  ]
}
```
