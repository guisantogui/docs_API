## Assinatura do Endpoint

POST - posts/{id}/report

## Descrição do negócio
Criar um _report_ sobre determinada postagem.

## Parametros na URL
id - Identificador da postagem

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
```
{
  "description": "string",
  "postReportOptionId": "00000000-0000-0000-0000-000000000000"
}
```

##Objeto de retorno

```
{
  "response": "00000000-0000-0000-0000-000000000000"
}
```