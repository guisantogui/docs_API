## Assinatura do Endpoint

GET - cms/talks/

## Descrição do negócio
Endpoint lista todas entidades do backend, respeitando os filtros e ordenado por:
1. Evento - propriedade Title na lingua portuguesa
2. Data Inicio - DESC (Mais ao futuro primeiro)
3. Sala - ASC - na lingua portuguesa

A busca devera respeitar as seguintes regras na busca:

- Datas
  - Data Inicio - pesquisar todas talks a partir da data
  - Data Fim - pesquisar todas talks a até da data
OBS: Caso ambos estejam preenchidos, filtrar o período


## Parametros na URL

####Parametros em via query
- title - filtra talk pelo seu titulo (Campo PT)
- category - filtro deve ser no campo title da tabela de traduções
- room - filtro deve ser no campo title da tabela de traduções
- active - filtra apenas talks ativas ou inativas
- eventId - filtra talks vinculadas no evento selecionado, ou nenhum
- autolike - filtra talks com autolike, sem autolike, ou ambos
- featuredColor - filtra talks com destaque, sem destaque, ou ambos
- carouselId - filtra talks vinculadas no carousel selecionado, ou nenhum
- speakerId - filtra talks vinculadas àquele palestrante selecionado, ou nenhum
- [Parâmetros de paginação](/API-\(Endpoints\)/Parâmetros-de-paginação)

OBS: Envio de booleanos que podem ser "ambos" com base nos [Parâmetros para consultas com boolean](/API-\(Endpoints\)/Parâmetros-para-consultas-com-boolean)

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": [
    {
      "title": "Talk 1", // registro em portugues
      "event": "Evento X", 
      "startDate": "15/12/2019 15:00:00",
      "endDate": "15/12/2019 16:00:00",
      "room": "Sala 1", // registro em portugues
      "category": "Category 1", // registro em portugues
      "active": true
    },
    {
      "title": "Talk 1", // registro em portugues
      "event": "Evento Y", 
      "startDate": "15/12/2019 15:00:00",
      "endDate": "15/12/2019 16:00:00",
      "room": "Sala 1", // registro em portugues
      "category": "Category 1", // registro em portugues
      "active": true
    }
    ]
}
```