## Assinatura do Endpoint

PUT - cms/interactives/

## Descrição do negócio
Endpoint deve persistir as alterações no objeto e seus vínculos no banco de dados, e deve dar o retorno apenas quando o objeto estiver persistido.

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
```
{
  "id": "444444444-888888888-9999999",
  "question": "grupo interativa",
  "time": 10,
  "order": 1,
  "typeId": "444444444-888888888-9999999",
  "groupId": "444444444-888888888-9999999", // <-- OU NULL
  "answerOptions": ["444444444-888888888-9999999", "444444444-888888888-9999999", 
"444444444-888888888-9999999"]
}
```

##Objeto de retorno

```
{
  "response": true
}
```