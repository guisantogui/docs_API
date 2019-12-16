## Assinatura do Endpoint

POST - cms/speakers/

## Descrição do negócio
Endpoint deve persistir um novo objeto e seus vínculos no banco de dados, e deve dar o retorno apenas, quando o objeto estiver persistido.

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

Até 1 arquivos binários (Imagem da postagem, enviado como Multipart header)
- Photo

Json: Texto da postagem, enviada string com encoding = "x-www-form-urlencoded" no formato json abaixo:

```
{
    "id": null,
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
     ]
}
```

##Objeto de envio
Não há

##Objeto de retorno

```
{
  "response": true
}
```