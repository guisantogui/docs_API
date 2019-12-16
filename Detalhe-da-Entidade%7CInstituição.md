## Assinatura do Endpoint

GET - /cms/institutions/{id}

## Descrição do negócio
Lista entidade de acordo com o ID

## Parametros na URL
id - identificador da entidade

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response":
    {
      "id": "00000000-0000-0000-0000-000000000000",
      "name": "string",
      "whiteLabelType": 1,
      "acronym": "str", // not null, valor default ""
      "dashboardEmail": "email@email.com", // not null, valor default ""
      "institutionEmail": "email@email.com", // not null, valor default ""
      "associationLink": "", // not null, valor default ""
      "active": true // not null, valor default true
    }
}
```