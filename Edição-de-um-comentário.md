## Assinatura do Endpoint

PUT - cms/comments/

## Descrição do negócio
Endpoint deve persistir um novo objeto e seus vínculos no banco de dados, e deve dar o retorno apenas, quando o objeto estiver persistido.
Lembrando que tanto usuário como postagem podem ser re-vinculados nesse endpoint.

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
```
{
    "id": null,
    "text": "Meu comentário",
    "userId": "888998-5454-548488-4545454",
    "postId": "888998-5454-548488-4545454"
}
```

##Objeto de retorno

```
{
  "response": true
}
```