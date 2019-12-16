## Assinatura do Endpoint

POST - cms/interactiveOptions/

## Descrição do negócio
Endpoint que cria uma nova entidade, e retorna se a criação foi feita com sucesso.

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
```
{
  "description": "grupo interativa",
  "order": 2,
  "isRight": true,
  "InteractiveId": "00000000000000-0000000000-0000" //<-- OU NULL
}
```

##Objeto de retorno

```
{
  "response": true
}
```