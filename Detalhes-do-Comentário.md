## Assinatura do Endpoint

GET - cms/comments/{id}

## Descrição do negócio
Endpoint lista as informações de determinado comentário

## Parametros na URL
id - identificador do comentário

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": [
    {
      "id": "988794564896-4856489-55120",
      "text": "",
      "userEmail": "",
      "verified": true,
      "postagem": "Texto da postagem a qual pertence",
      "event": {
        "id": "988794564896-4856489-55120",
        "name": "SOCERGS"
      },
      "institution": null
    },
    {
      "id": "988794564896-4856489-55120",
      "text": "",
      "userEmail": "",
      "verified": true,
      "postagem": "Texto da postagem a qual pertence",
      "event": null,
      "institution": {
        "id": "988794564896-4856489-55120",
        "name": "SOCERGS"
      }
    }
  ]
}
```