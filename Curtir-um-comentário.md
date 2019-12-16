## Assinatura do Endpoint

POST - posts/{id}/comments/{commentId}/likes

## Descrição do negócio
Endpoint responsável curtir um comentário para o usuário que está fazendo a requisição. Caso já houver uma curtida para aquele usuário deve somente ignorar a requisição.

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
  "response": "00000000-0000-0000-0000-000000000000"
}
```