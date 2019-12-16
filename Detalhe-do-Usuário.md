## Assinatura do Endpoint
GET - Users/{id}

## Descrição do negócio
Endpoint busca as informações do usuário

## Parametros na URL
id - Identificador do usuário

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": {
    "id": "00000000-0000-0000-0000-000000000000",
    "email": "string",
    "name": "string",
    "phoneNumber": "string",
    "enterpriseInstitution": "string",
    "jobTitle": "string",
    "description": "string",
    "profilePictureUrl": "string"
  }
}
```