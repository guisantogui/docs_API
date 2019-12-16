## Assinatura do Endpoint

POST - cms/setQuestionChoices/

## Descrição do negócio
Endpoint responsável por criar uma opção de pergunta de avaliação de set, não serão criados vínculos nessa criação.

## Parametros na URL

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
```
{
  "choice": "Uma escolha",
  "order": 8,
  "isRight": true
}
```

##Objeto de retorno

```
{ "response": true }
```