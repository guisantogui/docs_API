## Assinatura do Endpoint

POST - cms/eventRatingQuestions

## Descrição do negócio
Cria uma nova pergunta vinculada ao evento

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
```
{
  "questionPT": "title do evento PT",
  "questionES": "title do evento ES",
  "questionEN": "title do evento EN",
  "order": 8,
  "event": "98765457689-0987657890-0987657890" // não nullable
}
```

##Objeto de retorno
```
{
  "response":  true
}
```
