## Assinatura do Endpoint

POST - cms/generalInfos/

## Descrição do negócio
Endpoint que cria uma entidade (generalInfo) e seus vinculos no banco de dados.

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

Até 3 arquivos binários (Imagem da postagem, enviado como Multipart header)

- imagePT
- imageES
- imageEN

Json: Texto da postagem, enviada string com encoding = "x-www-form-urlencoded" no formato json abaixo:

```
{
  "id": null,
  "titlePT": "generalInfo",
  "titleES": "generalInfo",
  "titleEN": "generalInfo",
  "descriptionPT": "Informação Geral",
  "descriptionEN": "Informação Geral",
  "descriptionES": "Informação Geral",
  "type": "855852489648-5548858555-98988999",
  "formatAsHtml": true,
  "order": 2,
  "active": true,
  "events": [ "855852489648-5548858555-98988999", "855852489648-5548858555-98988999" ],
  "institutions": [ "855852489648-5548858555-98988999", "855852489648-5548858555-98988999" ]
}
```


##Objeto de envio
Não há

##Objeto de retorno

```
{
  "response": true
}
```