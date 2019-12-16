## Assinatura do Endpoint
GET - event/{id}/hasSubscription/{email}

## Descrição do negócio
Problema: O usuário não conseguir fazer o credenciamento pelo app, por que ele pode logar no app com um email diferente do utilizado na hora de fazer a inscrição no evento, portanto precisamos dar uma opção para que ele possa buscar os dados de credenciamento.

Solução: O endpoint deverá ser responsável por buscar as informações de credenciamento do usuário, a regra deverá ser a mesma do endpoint de listagem de eventos na sua V2.
Caso exista informação na coluna AccreditationDefaultContent da tabela Event, deverá ser feito a concatenação com o ExternalId da tabela SubscriptionIntegration.
A concatenação deverá ser feita no formato: string.Format(AccreditationDefaultContent, ExternalId)


## Parametros na URL
Não se aplica

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não há

##Objeto de retorno

```
{
   "response": "QRCODE DATA"
}
```