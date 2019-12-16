## Assinatura do Endpoint

PUT - cms/institutions/

## Descrição do negócio
Endpoint que edita uma entidade existente, e retorna se a edição foi feita com sucesso.

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
```
{
      "id": "8888888754612894568456"
      "title": "Titulo",
      "acronym": "Tit",
      "dashboardAcess": "emailAcesso@makadu.net",
      "active": true,
      "email": "socergs@socergs.com",
      "associationLink": "www.socergs.com/associese",
      "timelineType": "8888888-99999999-9888888888-5555"

```

##Objeto de retorno

```
{
  "response": true
}
```