## Assinatura do Endpoint

GET - cms/sets/{id}

## Descrição do negócio
Endpoint que busca os detalhes de um set

## Parametros na URL
id - Identificador do paper

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
      "description": "Descrição",
      "order": 8,
      "minRating": 4.5,
      "papers": [
        {
          "id": "55558-99999999-888888-66666",
          "name": "Nome do paper"
        },
        {
          "id": "55558-99999999-888888-66666",
          "name": "Nome do paper"
        }
      ],
      "questions": [
        {
          "id": "55558-99999999-888888-66666",
          "name": "Question 1"
        },
        {
          "id": "55558-99999999-888888-66666",
          "name": "Question 2"
        }
      ]
    },
    {
      "id": "988794564896-4856489-55120",
      "description": "Descrição",
      "order": 8,
      "minRating": 4.5,
      "papers": [
        {
          "id": "55558-99999999-888888-66666",
          "name": "Nome do paper"
        }
      ],
      "questions": [
        {
          "id": "55558-99999999-888888-66666",
          "name": "Question 1"
        }
      ]
    }
  ]
}
```