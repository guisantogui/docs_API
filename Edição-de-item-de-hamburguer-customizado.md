## Assinatura do Endpoint

PUT - cms/hamburguerCustom

## Descrição do negócio
Edita um item de hamburguer customizado, vinculado, poderá ser feito vinculo em outro item base.

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
```
{
  "id": "98765457689-0987657890-0987657890",
  "baseItem": "98765457689-0987657890-0987657890",
  "customLabelPT": "title do evento PT",
  "customLabelES": "title do evento ES",
  "customLabelEN": "title do evento EN",
  "order": 8,
  "active": false
}
```

##Objeto de retorno
```
{
  "response":  true
}
```
