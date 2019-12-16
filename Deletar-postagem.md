## Assinatura do Endpoint

DELETE - posts/{id}

## Descrição do negócio
Endpoint deve deletar a postagem do usuário, bem como todas suas dependências:
- likes
- comentários
- especializações (pinado, premium, agendado ...)
- biblioteca

Restrições:
- Uma postagem somente pode ser deletada pelo usuário que criou ela OU por um usuário verificado.

## Parametros na URL
id - Identificador da postagem

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