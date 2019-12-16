## Assinatura do Endpoint
GET - cms/users/{id}

## Descrição do negócio
Endpoint deve retornar o objeto referente ao Id enviado por parâmetro

## Parametros na URL
id - identificador do usuário

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)


##Objeto de envio
Não há

##Objeto de retorno

```
{
  "response": [
    {
      "id": "88878787878787815-4551-45454-5154",
      "name": "Nome",
      "email": "asdasdasd",
      "verifiedUser": true,
      "active": true,
      "phone": "55558855",
      "photoUrl: "http://image.com/png.png",
      "enterprise": "Makadu",
      "presentation": "Eu gosto de eventos",
      "events": [
        {
          "id": "454545487878-55445454-89898954-88855",
          "title": "SOCERGS"
        },
        {
          "id": "454545487878-55445454-89898954-88855",
          "title": "ENDIPE"
        }
      ],
      "EvaluationPapers": [
        {
          "id": "454545487878-55445454-89898954-88855",
          "title": "A importancia da Tecnologia na saúde"
        }      
      ]
    }
  ]
}
```