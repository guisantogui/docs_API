## Assinatura do Endpoint

DELETE - cms/sets/{id}

## Descrição do negócio
Endpoint deve remover o objeto do set, caso existam os vínculos com opções, deve remover os vínculos, e também caso existam respostas limpar as respostas também.

## Parametros na URL
id - identificador do comentário

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não há

##Objeto de retorno

```
{
  "response": true
}
```