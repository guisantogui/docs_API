
## Assinatura do Endpoint
GET - events/{id}/participants

## Descrição do negócio
Endpoint que lista todos os participantes que adicionaram o evento aos "Meus eventos"

## Parametros na URL
id - Identificador do evento

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": [
    {
      "qntyUnreadMessages": 0,
      "id": "string",
      "name": "string",
      "jobTitle": "string",
      "profilePictureUrl": "string"
    }
  ]
}
```
