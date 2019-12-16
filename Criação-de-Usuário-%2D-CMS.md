## Assinatura do Endpoint
POST - cms/users

## Descrição do negócio
Cria um novo usuário
A criação do usuário deverá verificar se o email do usuário existe na tabela UserEvaluatorPaper, tabela que liga os Usuários avaliadores a seus Papers, e caso o email exista com Id de usuário Nulo, a coluna de Id de Usuário deverá ser preenchida, caso não exista, a funcionalidade não deve ser alterada.

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
      "name": "texto da postagem",
      "email": "asdasdasd",
      "verifiedUser": true,
      "active": true,
      "phone": "55558855",
      "enterprise": "Makadu",
      "description": "Eu gosto de eventos",
      "events": [
         "454545487878-55445454-89898954-88855",
         "454545487878-55445454-89898954-88855",
         "454545487878-55445454-89898954-88855"
      ],
      "evaluationPapers": [
        "55558882211446555-878989887-897897897-87987"
      ]
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