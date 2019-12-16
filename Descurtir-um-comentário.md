## Assinatura do Endpoint

DELETE /api/posts/{id}/comments/{commentId}/likes

## Descrição do negócio
Endpoint responsável descurtir um comentário para o usuário que está fazendo a requisição. Caso não houver uma curtida para aquele usuário deve somente ignorar a requisição.

## Parâmetros na URL
id - Identificador da postagem
commentId - Identificador do comentário

##Parâmetros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": true
}
```