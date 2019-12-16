## Assinatura do Endpoint

PUT - cms/paper/

## Descrição do negócio
Endpoint deve persistir as atualizações do objeto bem como seus vínculos no banco de dados, e deve dar o retorno apenas, quando o objeto estiver persistido.

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

Até 1 arquivos binários (poster do paper, enviado como Multipart header)
- poster

Json: Texto da postagem, enviada string com encoding = "x-www-form-urlencoded" no formato json abaixo:

##Objeto de envio
```
{
    "id": "000987890=937895-486384-8737383",
    "titlePT": "titulo da langauge",
    "titleEN": "titulo da langauge",
    "titleES": "titulo da langauge",
    "abstractPT": "abstract da langauge",
    "abstractEN": "abstract da langauge",
    "abstractES": "abstract da langauge",
    "categoryPT": "category da langauge",
    "categoryEN": "category da langauge",
    "categoryES": "category da langauge",
    "presentationPlacePT": "place da langauge",
    "presentationPlaceEN": "place da langauge",
    "presentationPlaceES": "place da langauge",
    "uniqueId": "98-09",
    "institutionName": "nome",
    "subjectPT": "",
    "subjectEN": "",
    "subjectES": "",
    "presentationStartDate": "20191215185255",
    "presentationEndDate": "20191215190255",
    "mainAuthor": "Nome do autor principal",
    "eventId": "000987890=937895-486384-8737383",
    "sets": [ "000987890=937895-486384-8737383",  "000987890=937895-486384-8737383", "000987890=937895-486384-8737383"],
    "removePoster": false
}
```

##Objeto de retorno

```
{
  "response": true
}
```