## Assinatura do Endpoint

POST /api/posts/{id}/likes

## Descrição do negócio
Endpoint responsável curtir uma postagem para o usuário que está fazendo a requisição. Caso já houver uma curtida para aquele usuário deve somente ignorar a requisição.

## Parâmetros na URL
id - Identificador da postagem

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