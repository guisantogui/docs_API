## Assinatura do Endpoint

POST - talks/{id}/ratings

## Descrição do negócio
Avaliação simples de estrelas da palestra.

## Parametros na URL
id - Identificador da palestra 

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
```
{
  "rating": 0,
  "comment": "string"
}
```

##Objeto de retorno

```
{
  "response": true
}
```