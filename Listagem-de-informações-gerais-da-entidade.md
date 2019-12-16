## Assinatura do Endpoint

GET - institutions/{id}/general_infos/{typeId}

## Descrição do negócio
Listagem das informações gerais de determinado tipo, da entidade

## Parametros na URL
id - identificador da entidade
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