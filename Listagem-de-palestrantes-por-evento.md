## Assinatura do Endpoint

GET - events/{id}/speakers

## Descrição do negócio
Endpoint que lista todos palestrantes do evento

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
      "about": "string",
      "cpf": "string",
      "email": "string",
      "profilePictureUrl": "string",
      "id": "00000000-0000-0000-0000-000000000000",
      "name": "string"
    }
  ]
}
```