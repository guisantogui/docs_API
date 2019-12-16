## Assinatura do Endpoint

DELETE /api/posts/{id}/likes

## Descrição do negócio
Endpoint responsável descurtir uma postagem para o usuário que está fazendo a requisição. Caso não houver curtida para aquele usuário deve somente ignorar a requisição.

## Parametros na URL
id - Identificador da postagem

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": true
}
```