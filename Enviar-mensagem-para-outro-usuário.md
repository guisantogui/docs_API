## Assinatura do Endpoint

POST - users/{id}/message

## Descrição do negócio
Endpoint que envia mensagens de um usuário para outro

## Parametros na URL
id - identificador do usuário

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
```
{
  "response": true
}
```

##Objeto de retorno

```
{
  "messageBody": "string"
}
```