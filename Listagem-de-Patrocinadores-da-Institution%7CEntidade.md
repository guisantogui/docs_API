## Assinatura do Endpoint

GET - institution/{id}/sponsors

## Descrição do negócio
Listagem de todos patrocinadores da entidade

## Parametros na URL
id - identificador da entidade

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": [
    {
      "id": "00000000-0000-0000-0000-000000000000",
      "name": "string",
      "bannerPictureUrl": "string"
    }
  ]
}
```