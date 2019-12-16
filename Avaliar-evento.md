
## Assinatura do Endpoint

POST - events/{id}/rating

## Descrição do negócio
Cria ou atualizar uma avaliação do evento daquele usuário

## Parametros na URL
id - Identificador do evento

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio

```
[
  {
    "questionId": "00000000-0000-0000-0000-000000000000",
    "textAnswer": "string",
    "rating": 0
  }
]
```

##Objeto de retorno

```
{
  "response": true
}
```
