## Assinatura do Endpoint

GET - cms/institutions/

## Descrição do negócio
Endpoint lista todas entidades do backend, respeitando os filtros e ordenado por:
1. Acronym
2. Title

## Parametros na URL

####Parametros em via query
- title
- acronym
- dashboardAcess (Email acesso)
- active - somente aparecerá entidades ativas, ou inativas, nunca ambas
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
      "title": "Titulo",
      "acronym": "Tit",
      "dashboardEmail": "emailAcesso@makadu.net",
      "active": true,
      "institutionEmail": "socergs@socergs.com",
      "associationLink": "www.socergs.com/associese",
      "timelineType": {
        "id": "8888888-99999999-9888888888-5555",
        "name": "Tipo 1"
      }
    },
    {
      "title": "Titulo",
      "acronym": "Tit",
      "dashboardEmail": "emailAcesso@makadu.net",
      "active": true,
      "institutionEmail": "socergs@socergs.com",
      "associationLink": "www.socergs.com/associese",
      "timelineType": {
        "id": "8888888-99999999-9888888888-5555",
        "name": "Tipo 1"
      }
    }
    ]
}
```