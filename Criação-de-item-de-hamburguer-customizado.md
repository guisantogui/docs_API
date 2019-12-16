## Assinatura do Endpoint

POST - cms/hamburguerCustom

## Descrição do negócio
Cria um novo item de hamburguer customizado, vinculado à um evento ou entidade.

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
```
{
  "baseItem": "98765457689-0987657890-0987657890",
  "customLabelPT": "title do evento PT",
  "customLabelES": "title do evento ES",
  "customLabelEN": "title do evento EN",
  "order": 8,
  "active": false,
  "event": "98765457689-0987657890-0987657890", //nullable
  "institution": "98765457689-0987657890-0987657890" //nullable
}
```

##Objeto de retorno
```
{
  "response":  true
}
```
