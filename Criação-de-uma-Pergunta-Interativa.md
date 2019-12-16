## Assinatura do Endpoint

POST - cms/interactives/

## Descrição do negócio
Endpoint que cria uma nova entidade, e retorna se a criação foi feita com sucesso.

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
```
{
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