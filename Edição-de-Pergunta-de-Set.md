## Assinatura do Endpoint

PUT - cms/setQuestions/

## Descrição do negócio
Endpoint para persistência das atualizações do objeto do RatingSetQuestion, bem como vínculos com as suas choices, removendo atuais ou inculindo novos.

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio

```
{
    "id": "988794564896-4856489-55120",
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