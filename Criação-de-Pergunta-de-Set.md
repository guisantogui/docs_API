## Assinatura do Endpoint

POST - cms/setQuestions/

## Descrição do negócio
Endpoint para persistência de um objeto do RatingSetQuestion, bem como vínculos com as suas choices.

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
```
{
    "question": "Texto da pergunta",
    "typeId": "988794564896-4856489-55120",
    "choices": ["988794564896-4856489-55120", "988794564896-4856489-55120"],
    "order": 0
}
```

##Objeto de retorno

```
{
    "response": true
}
```