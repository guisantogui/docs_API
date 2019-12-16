## Assinatura do Endpoint

POST - cms/institutions/

## Descrição do negócio
Endpoint que cria uma nova entidade, e retorna se a criação foi feita com sucesso.

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
```
{
      "id": null
      "title": "Titulo",
      "acronym": "Tit",
      "dashboardEmail": "emailAcesso@makadu.net",
      "active": true,
      "institutionEmail": "socergs@socergs.com",
      "associationLink": "www.socergs.com/associese",
      "timelineType": 1
}
```

##Objeto de retorno

```
{
  "response": true
}
```