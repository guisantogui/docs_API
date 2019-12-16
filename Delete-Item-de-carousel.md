## Assinatura do Endpoint

DELETE - cms/carousel/{id}

## Descrição do negócio
Endpoint que deleta o item do carousel, obviamente removendo vinculos, com evento, entidade, ou grupo de carousel.

Caso ele tenha mídia vinculada a ele, deve remover os objetos em cascata.
Caso tenha, palestrante, palestra, patrocinador, grupo de interativa, não deve remover nenhum desses objetos.

## Parametros na URL
id - Identificador do item de carousel

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