## Assinatura do Endpoint

GET - cms/carousel/

## Descrição do negócio
Endpoint lista todas entidades do backend, respeitando os filtros e ordenado por:
1. Evento (não considerar itens ligados em grupos), propriedade TitlePT
2. Entidade, propriedade Name
3. Description

## Parametros na URL

####Parametros em via query
- description - filtra itens pela descrição
- event - filtra somente itens do evento descrito, filtro deve ser no campo title da tabela de traduções
- startDate - filtra itens a partir daquela data
- endDate - filtra itens até aquela data
- group - filtra itens vinculados ao grupo, filtro deve ser no campo name
- [Parâmetros de paginação](/API-\(Endpoints\)/Parâmetros-de-paginação)

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": [
    {
      "id": "55454564654-5465484564-54464534",
      "description": "item X",
      "event": "evt",
      "institution": "name",
      "tyoe": "link/biblioteca/sponsor/palestrante/palestra/interativa",
      "thumbnail": "http://www.makaduapi.com/photo2.jpg",
      "active": true,
      "startDate": "13/12/2019 18:00:00",
      "endDate": "13/12/2019 19:00:00"
    },
    {
      "id": "55454564654-5465484564-54464534",
      "description": "item X",
      "event": "evt",
      "institution": "name",
      "tyoe": "link/biblioteca/sponsor/palestrante/palestra/interativa",
      "thumbnail": "http://www.makaduapi.com/photo2.jpg",
      "active": true,
      "startDate": "13/12/2019 18:00:00",
      "endDate": "13/12/2019 19:00:00"
    }
    ]
}
```