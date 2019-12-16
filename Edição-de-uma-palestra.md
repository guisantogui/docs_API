## Assinatura do Endpoint

PUT - cms/talk/

## Descrição do negócio
Endpoint deve persistir as alterações no objeto e seus vínculos (e exclusões de vínculos) no banco de dados, e deve dar o retorno apenas, quando o objeto estiver persistido.

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
```
{
    "id": "5555555-888888-5454545-55555",
    "titlePT": "Makadu",
    "titleEN": "Titulo EN",
    "titleES": "Titulo ES",
    "descriptionPT": "Description",
    "descriptionEN": "Description",
    "descriptionES": "Description",
    "roomPT": "Description",
    "roomEN": "Description",
    "roomES": "Description",
    "categoryPT": "Description",
    "categoryEN": "Description",
    "categoryES": "Description",
    "startDate": "20190205100000", // No formato: yyyyMMddHHmmss
    "endDate": "20190205110000", // No formato: yyyyMMddHHmmss
    "eventId": "5555555-888888-5454545-55555",
    "carousels": [
         "5555555-888888-5454545-55555",
         "5555555-888888-5454545-55555",
         "5555555-888888-5454545-55555"
     ],
    "active": true,
    "autolike": false,
    "featuredColor": "#888855",
    "speakers": [
         "5555555-888888-5454545-55555",
         "5555555-888888-5454545-55555",
         "5555555-888888-5454545-55555"
     ],
     "ratingQuestions": [
         {
             "id": "5555555-888888-5454545-55555",
             "question": "Pergunta"
         },
         {
             "id": null,
             "question": "Nova Pergunta"
         }]
     
}
```

##Objeto de retorno

```
{
  "response": true
}
```