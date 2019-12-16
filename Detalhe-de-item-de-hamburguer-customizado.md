## Assinatura do Endpoint

GET - cms/hamburguerCustom/{id}

## Descrição do negócio
Lista os detalhes de um item de hamburguer

## Parametros na URL
id - identificador do item de hamburguer customizado

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": {
    "id": "988794564896-4856489-55120",
    "baseItem": {
      "id": "98765457689-0987657890-0987657890",
      "name": "Uma escolha"
    },
    "customLabelPT": "title do evento PT",
    "customLabelES": "title do evento ES",
    "customLabelEN": "title do evento EN",
    "order": 8,
    "active": true,
    "event": {
      "id": "98765457689-0987657890-0987657890",
      "name": "socergs 2019"
    },
    "institution": {
      "id": "98765457689-0987657890-0987657890",
      "name": "socergs"
    }
  }
}
```