## Assinatura do Endpoint

DELETE - cms/whitelabel/{id}

## Descrição do negócio
Deleta o White label e os vinculos existentes no banco de dados, o retorno somente deve ser dado, após a persistência da exclusão.

## Parametros na URL
id - identificador do white label que será excluído

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": true
}
```