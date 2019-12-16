## Assinatura do Endpoint
GET - events/{id}/notifications

## Descrição do negócio
Endpoint que lista as notificações do usuário, que podem levar o usuário para uma postagem, ou palestra.

## Parametros na URL
id - Identificador do evento

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": {
    "total": 0,
    "notifications": [
      {
        "id": "00000000-0000-0000-0000-000000000000",
        "notificationType": 1,
        "userIdAction": "string",
        "actionOriginName": "string",
        "dateCreated": "2018-11-19T13:01:25.330Z",
        "seen": true,
        "talkId": "00000000-0000-0000-0000-000000000000",
        "postId": "00000000-0000-0000-0000-000000000000",
        "commentId": "00000000-0000-0000-0000-000000000000"
      }
    ]
  }
}
```