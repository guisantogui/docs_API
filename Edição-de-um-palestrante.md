## Assinatura do Endpoint

PUT - cms/speakers/

## Descrição do negócio
Endpoint deve persistir as alterações no objeto e seus vínculos (criação ou remoção) no banco de dados, e deve dar o retorno apenas, quando o objeto estiver persistido.

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

Até 1 arquivos binários (Imagem da postagem, enviado como Multipart header)
- Photo

1 arquivo json: Texto da postagem, enviada string com encoding = "x-www-form-urlencoded" no formato json abaixo:

```
{
    "id": "5555555-888888-5454545-55555",
    "name": "Makadu",
    "cpf": "55558888945",
    "email": "Makadu@makadu.net",
    "aboutPT": "Description",
    "aboutEN": "Description",
    "aboutES": "Description",
    "talks": [
         "5555555-888888-5454545-55555",
         "5555555-888888-5454545-55555",
         "5555555-888888-5454545-55555"
     ],
     "removePhoto": false

}
```

##Considerações especiais
- Sobre o atributo `removePhoto`:
  - Ele controlará a exclusão de uma foto pré-existente.
  - O speaker somente terá uma foto removida quando essa propriedade for verdadeira.
  - Sempre que a flag vier com valor verdadeiro, o usuário deverá ficar sem nenhuma foto, após a persistência dos dados.
  - Caso a flag venha com valor false, e nenhum objeto de foto, nada referente a foto deverá ser feito, ou seja, manter a anterior, ou manter o speaker sem foto.

##Objeto de envio
Não há

##Objeto de retorno

```
{
  "response": true
}
```