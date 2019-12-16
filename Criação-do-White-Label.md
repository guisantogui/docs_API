## Assinatura do Endpoint

POST - cms/whitelabel/

## Descrição do negócio
Endpoint deve persistir um novo objeto no banco de dados, e deve dar o retorno apenas, quando o objeto estiver persistido.

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
```
{
    "id": null,
    "title": "Makadu",
    "type": "00000-545454-0000-5454545",
    "linkIOs": "http://appstore.com/makadu",
    "linkAndroid": "http://playstore.com/makadu",
    "institutionId": "000000-0000000-000000000" //ou null
}
```

##Objeto de retorno

```
{
  "response": true
}
```