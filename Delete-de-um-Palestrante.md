## Assinatura do Endpoint

DELETE - cms/speakers/{id}

## Descrição do negócio
Endpoint deve remover o objeto e seus vínculos no banco de dados, e deve dar o retorno apenas, quando o objeto estiver persistido.
Vínculos:
- Carousel
- Palestra
- Tabela de linguagem do palestrante

Importante apenas os vínculos são removidos.

## Parâmetros na URL
id - Identificador do palestrante

##Parâmetros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não há

##Objeto de retorno

```
{
  "response": true
}
```