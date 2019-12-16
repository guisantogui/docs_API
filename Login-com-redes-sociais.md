## Assinatura do Endpoint

POST - users/socialLogin

## Descrição do negócio
Endpoint responsável por fazer login com as redes sociais, com Google ou Facebook.
O login deverá verificar se o email do usuário existe na tabela AspNetUsersPapers, tabela que liga os Usuários avaliadores a seus Papers, e caso o email exista com Id de usuário Nulo, a coluna de Id de Usuário deverá ser preenchida, caso não exista, a funcionalidade não deve ser alterada.

## Parametros na URL
Não se aplica

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
```
{
  "name": "string",
  "email": "string",
  "id": "string",
  "socialNetworkType": 1,
  "profilePictureUrl": "string"
}
```

##Objeto de retorno
```
{
  "response": {
    "verified": true,
    "socialNetworks": [
      {
        "id": "string",
        "name": "string"
      }
    ],
    "roles": [
      {
        "roleId": "string",
        "name": "string"
      }
    ],
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