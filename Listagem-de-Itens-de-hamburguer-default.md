## Assinatura do Endpoint

GET - cms/hamburguerDefault/

## Descrição do negócio
Endpoint lista todas as opções de item de hamburguer presentes na tabela HamburguerItem, combinada com HamburguerItemLanguage, retornar apenas o label em Português, ordenar pela "order".

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": [
    {
      "id": "988794564896-4856489-55120",
      "name": "Conteúdo"
    },
    {
      "id": "988794564896-4856489-55120",
      "name": "Programação"
    }
  ]
}
```