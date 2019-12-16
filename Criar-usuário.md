## Assinatura do Endpoint
POST - Users

## Descrição do negócio
Cria um novo usuário
A criação do usuário deverá verificar se o email do usuário existe na tabela UserEvaluatorPaper, tabela que liga os Usuários avaliadores a seus Papers, e caso o email exista com Id de usuário Nulo, a coluna de Id de Usuário deverá ser preenchida, caso não exista, a funcionalidade não deve ser alterada.


## Parametros na URL
Não se aplica

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
```
{
  "password": "string",
  "id": "00000000-0000-0000-0000-000000000000",
  "email": "string",
  "name": "string",
  "phoneNumber": "string",
  "enterpriseInstitution": "string",
  "jobTitle": "string",
  "description": "string",
  "profilePictureUrl": "string"
}
```

##Objeto de retorno

```
{}
```