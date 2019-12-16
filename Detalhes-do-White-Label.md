## Assinatura do Endpoint

GET - cms/whitelabels/{id}
GET - api/whitelabels/{id} <-- Endpoint para atender aos apps

## Descrição do negócio
Retorna as informações do white label, será utilizado para definição do tipo de aplicativo que será apresentado ao usuário.

## Parametros na URL
id - identificador do white label

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": {
    "id": "0000000-0000000-000000000",
    "title": "Makadu",
    "typeId": 1,
    "linkIOs": "http://appstore.com/makadu",
    "linkAndroid": "http://playstore.com/makadu",
    "institution": { /*ou null*/
      "id": "000000-0000000-000000000",
      "title": "Titulo",
      "timelineType": 1
    } 
  }
}
```