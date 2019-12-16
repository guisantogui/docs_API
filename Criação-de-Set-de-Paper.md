## Assinatura do Endpoint

POST - cms/sets/

## Descrição do negócio
Endpoint deve persistir um novo objeto e seus vínculos no banco de dados, e deve dar o retorno apenas, quando o objeto estiver persistido.
É possível vincular o set em papers na sua criação, e também vincular perguntas já criadas no Set.

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
```
{
  "description": "Descrição",
  "order": 1,
  "MinRating": 8.9,
  "papers": [
    "555888-9999665-8455412-62225",
    "555888-9999665-8455412-62225",
    "555888-9999665-8455412-62225"
  ],
  "questions": [
    "555888-9999665-8455412-62225",
    "555888-9999665-8455412-62225",
    "555888-9999665-8455412-62225"
  ]
}
```

##Objeto de retorno

```
{
  "response": true
}
```