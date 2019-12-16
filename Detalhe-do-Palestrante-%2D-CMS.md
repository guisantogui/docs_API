## Assinatura do Endpoint

GET - cms/speakers/{id}

## Descrição do negócio
Descrição das informações do palestrante.

## Parametros na URL
id - Identificador do palestrante

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": {
    "aboutPT": "string",
    "aboutEN": "string",
    "aboutES": "string",
    "cpf": "string",
    "email": "string",
    "profilePictureUrl": "string",
    "id": "00000000-0000-0000-0000-000000000000",
    "name": "string"
  }
}
```