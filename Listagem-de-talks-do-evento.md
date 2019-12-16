## Assinatura do Endpoint

GET - /events/{id}/talks

## Descrição do negócio
Endpoint que lista todas talks ativas do evento enviado por parâmetro

## Parametros na URL
id - identificador do evento

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio

NÂO SE APLICA


##Objeto de retorno

```
{
  "response": [
    {
      "category": "string",
      "subCategories": [
        {
          "startDate": "2018-11-19T13:01:25.129Z",
          "talks": [
            {
              "favorited": true,
              "speakers": [
                {
                  "about": "string",
                  "cpf": "string",
                  "email": "string",
                  "profilePictureUrl": "string",
                  "id": "00000000-0000-0000-0000-000000000000",
                  "name": "string"
                }
              ],
              "id": "00000000-0000-0000-0000-000000000000",
              "title": "string",
              "description": "string",
              "startDate": "2018-11-19T13:01:25.129Z",
              "endDate": "2018-11-19T13:01:25.129Z",
              "room": "string",
              "category": "string",
              "featuredColor": "string"
            }
          ]
        }
      ]
    }
  ]
}
```