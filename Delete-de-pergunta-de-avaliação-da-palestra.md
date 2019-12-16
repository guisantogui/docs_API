## Assinatura do Endpoint

DELETE - cms/talkRatingQuestion/{id}

## Descrição do negócio
Deleta a Entidade e vínculos existentes no banco de dados fisicamente, o retorno somente deve ser dado, após a persistência da exclusão.
Caso existam respostas para a pergunta deletada, as perguntas deverão ser deletadas também.

## Parametros na URL
id - identificador da pergunta que será excluída

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": true
}
```