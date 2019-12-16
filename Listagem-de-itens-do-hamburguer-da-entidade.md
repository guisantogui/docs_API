## Assinatura do Endpoint

GET - institution/{id}/hamburguerItens

## Descrição do negócio
Lista os itens de menu daquela entidade, somente itens ativos são listados, e itens personalizados já trazem seu label especial.

## Parametros na URL
id - Identificador da entidade

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": [
    {
      "id": "00000000-0000-0000-0000-000000000000",
      "label": "string",
      "order": 0,
      "notificationCount": 0
    }
  ]
}
```