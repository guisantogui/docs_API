## Assinatura do Endpoint

GET - cms/setQuestions/{id}

## Descrição do negócio
Endpoint que busca os detalhes de uma pergunta de avaliação de paper

## Parametros na URL
id - identificador da pergunta

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": {
    "id": "988794564896-4856489-55120",
    "question": "Texto da pergunta",
    "type": {
      "id": "988794564896-4856489-55120",
      "name": "Numerico"
    },
    "choices": [
      {
        "id": "988794564896-4856489-55120",
        "name": "Escolha"
      },
      {
        "id": "988794564896-4856489-55120",
        "name": "Escolha"
      }
    ]
  }
}
```