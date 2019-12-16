## Assinatura do Endpoint

POST - interactives/{id}/answer

## Descrição do negócio
Endpoint que envia a opção ou resposta textual do usuário para  a interativa

## Parametros na URL
id - identificador da pergunta interativa

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
```
{
  "answerText": "string",
  "answerOptionId": "00000000-0000-0000-0000-000000000000"
}
```

##Objeto de retorno

```
{
  "response": true
}
```