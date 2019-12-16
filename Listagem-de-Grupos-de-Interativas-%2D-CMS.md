## Assinatura do Endpoint

GET - cms/interactiveGroups/

## Descrição do negócio
Endpoint lista todas entidades do backend, respeitando os filtros e ordenado por:
1. Label Date - ASC
2. Evento - propriedade Title na lingua portuguesa

## Parametros na URL

####Parametros em via query
- name - filtra grupo de interativa pelo seu nome
- active - filtra apenas grupo de interativa ativos ou inativos
- labelDate - filtra grupos de interativas pelo seu labelDate
- place - filtra grupos de interativas pelo seu Place
- carouselId - filtra grupos de interativas vinculados no carousel selecionado, ou nenhum
- eventId - filtra grupos de interativas vinculados no evento selecionado, ou nenhum
- [Parâmetros de paginação](/API-\(Endpoints\)/Parâmetros-de-paginação)

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": [
    {
      "id": "444444444-888888888-9999999",
      "name": "grupo interativa",
      "labelDate": "Dia 10",
      "place": "sala 05",
      "event": {
        "id": "444444444-888888888-9999999",
        "title": "Titulo" //pegar do registro PT
      },
      "carousel": {
        "id": "444444444-888888888-9999999",
        "description": "carousel X"
      },
      "active": true
    },
    {
      "id": "444444444-888888888-9999999",
      "name": "grupo interativa",
      "labelDate": "Dia 10",
      "place": "sala 05",
      "event": {
        "id": "444444444-888888888-9999999",
        "title": "Titulo" //pegar do registro PT
      },
      "carousel": {
        "id": "444444444-888888888-9999999",
        "description": "carousel X"
      },
      "active": true
    }
  ]
}
```