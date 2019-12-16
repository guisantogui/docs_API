## Assinatura do Endpoint

PUT - cms/whitelabel/

## Descrição do negócio
Endpoint deve editar o objeto no banco de dados, lembrando que o vinculo com a institution possa ser desfeita, caso o box seja enviado com null, e deve dar o retorno apenas, quando o objeto estiver persistido.

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
```
{
    "id": "151545-00584545-0000000-000000000",
    "title": "Makadu",
    "type": 1,
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