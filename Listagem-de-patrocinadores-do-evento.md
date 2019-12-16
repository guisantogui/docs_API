## Assinatura do Endpoint

GET - events/{id}/sponsors

## Descrição do negócio
Listagem de todos patrocinadores do evento

## Parametros na URL
id - identificador do evento

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