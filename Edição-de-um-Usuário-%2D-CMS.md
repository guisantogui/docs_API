## Assinatura do Endpoint
PUT - cms/users

## Descrição do negócio
Edita um novo usuário existente, bem como vínculos com outros objetos, removendo ou adicionando novos.

## Parametros na URL
Não se aplica

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

Até 1 arquivos binários (Imagem da postagem, enviado como Multipart header)
- photo

Json: Texto da postagem, enviada string com encoding = "x-www-form-urlencoded" no formato json abaixo:
```
{
  "response": [
    {
      "id": null,
      "name": "texto da postagem",
      "email": "asdasdasd",
      "verifiedUser": true,
      "active": true,
      "phone": "55558855",
      "enterprise": "Makadu",
      "presentation": "Eu gosto de eventos",
      "events": [
         "454545487878-55445454-89898954-88855",
         "454545487878-55445454-89898954-88855",
         "454545487878-55445454-89898954-88855"
      ],
      "EvaluationPapers": [
        "55558882211446555-878989887-897897897-87987"
      ],
      "removePhoto": false
    }
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