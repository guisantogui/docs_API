## Assinatura do Endpoint
DELETE - cms/posts/{id}

## Descrição do negócio
Endpoint responsável por deletar FISICAMENTE uma postagem, sendo assim, o vinculo com a timeline e usuário a qual a postagem pertence deverá ser deletado.
Em cascata deverão ser deletados mídia, comentários e likes referentes a postagem.

## Parametros na URL
Não se aplica

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)


##Objeto de envio
Não há

##Objeto de retorno

```
{
   "response": true
}
```