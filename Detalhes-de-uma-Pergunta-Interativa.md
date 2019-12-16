## Assinatura do Endpoint

GET - cms/interactiveGroups/{id}

## Descrição do negócio
Endpoint deve trazer as informações da pergunta interativa, bem como suas opções de escolha
## Parametros na URL
id - identificador do grupo de interativa

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
Não há

##Objeto de retorno
```
{
  "id": "444444444-888888888-9999999",
  "question": "grupo interativa",
  "type": {
      "id": "444444444-888888888-9999999",
      "name": "Pergunta 2"
  },
  "time": 41,
  "groupId": {
      "id": "444444444-888888888-9999999",
      "name": "grupo 5"
   },
  "answerOptions": [
    {
      "id": "444444444-888888888-9999999",
      "name": "Pergunta 2"
    },
    {
      "id": "444444444-888888888-9999999",
      "name": "Pergunta 5"
    },
    {
      "id": "444444444-888888888-9999999",
      "name": "Pergunta 1"
    }
  ]
}
```