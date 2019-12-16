## Assinatura do Endpoint

GET - cms/carouselGroup/

## Descrição do negócio
Endpoint lista todas entidades do backend, respeitando os filtros e ordenado por:
1. Evento
2. Name

## Parametros na URL

####Parametros em via query
- name - filtra grupos pelo seu nome
- event - filtra somente grupos do evento descrita, filtro deve ser no campo title da tabela de traduções
- startDate - filtra itens a partir daquela data
- endDate - filtra itens até aquela data
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
      "name": "item X",
      "event": "evt",
      "startDate": "13/12/2019 18:00:00",
      "endDate": "13/12/2019 19:00:00",
      "cycleTime": 40
    },
    {
      "id": "55454564654-5465484564-54464534",
      "name": "item X",
      "event": "evt",
      "startDate": "13/12/2019 18:00:00",
      "endDate": "13/12/2019 19:00:00",
      "cycleTime": 40
    }
    ]
}
```