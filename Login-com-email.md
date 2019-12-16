## Assinatura do Endpoint

POST /api/users/login

## Descrição do negócio
Realiza o login no backend, ou nega o acesso.
Deverá passar a trazer as roles na qual o usuário está vinculado.
O login deverá verificar se o email do usuário existe na tabela AspNetUsersPapers, tabela que liga os Usuários avaliadores a seus Papers, e caso o email exista com Id de usuário Nulo, a coluna de Id de Usuário deverá ser preenchida, caso não exista, a funcionalidade não deve ser alterada.

## Parametros na URL
Não se aplica

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
```
{
  "email": "string",
  "password": "string"
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