## Assinatura do Endpoint

POST - posts/{id}/comments

## Descrição do negócio
Endpoint responsável por criar um novo comentário em qualquer postagem do backend, independente da timeline

## Parametros na URL
id - Identificador da postagem

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
```
{
  "text": "string"
}
```

##Objeto de retorno

```
{
  "response": "00000000-0000-0000-0000-000000000000"
}
```