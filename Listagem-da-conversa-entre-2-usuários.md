## Assinatura do Endpoint

GET - users/{id}/message

## Descrição do negócio
Listagem da conversa entre 2 usuários

## Parametros na URL
id - identificador do usuário

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": [
    {
      "id": "00000000-0000-0000-0000-000000000000",
      "userSenderId": "string",
      "userReceiverId": "string",
      "sentByMe": true,
      "dateSent": "2018-11-19T13:01:25.776Z",
      "messageBody": "string"
    }
  ]
}
```