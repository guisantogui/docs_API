## Assinatura do Endpoint

GET - events/{id}/general_infos/{typeId}

## Descrição do negócio
Listagem das informações gerais de determinado tipo

## Parametros na URL
id - identificador do evento
typeId - Tipo de informação geral buscada naquele endpoint, pode ser dos tipos:
 - Mapa
 - Regulamento
 - Aviso
 - FAQ

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
      "description": "string",
      "title": "string",
      "formatDescriptionAsHtml": true,
      "imageUrl": "string",
      "order": 0,
      "generalInfoTypeId": "00000000-0000-0000-0000-000000000000"
    }
  ]
}
```