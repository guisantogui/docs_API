## Assinatura do Endpoint

GET- api/events/{id}/timeline

## Descrição do negócio
Endpoint responsável por trazer as postagens na timeline do evento, tipos de postagens que são retornadas nesse endpoint:
- Post pinado, fica sempre em primeiro lugar nos apps, o post pinado tem uma data de pinagem e despinagem, na sua criação uma dessas datas pode ser nula, sendo assim a query deverá considerar o range quando fizer a consulta e trazer o primeiro post pinado dentro do range, lembrando que caso um post pinado tenha apenas a data de início ele virá sempre como pinado a partir daquela data.
- Post premium, background colorido
- Post agendado, só aparece a partir de determinada data
- Post de próximas atividades, lista talks que vão acontecer nos próximos minutos

## Parametros na URL
id - identificador do evento

####Parametros query
skip - valor inteiro que define o post atual para paginação, assim pulando a quantidade definida na hora de buscar na base de dados
take - valor inteiro que define a quantidade de posts buscados a cada paginação


##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio

Não se aplica

##Objeto de retorno

```
{
  "response": {
    "nextTalks": [
      {
        "id": "00000000-0000-0000-0000-000000000000",
        "title": "string",
        "startDate": "2018-11-19T13:01:25.196Z",
        "endDate": "2018-11-19T13:01:25.196Z",
        "room": "string",
        "favorited": true
      }
    ],
    "posts": [
      {
        "userVerified": true,
        "postType": 1,
        "medias": [
          {
            "dateCreated": "2018-11-19T13:01:25.196Z",
            "videoLength": "string",
            "mediaType": {
              "id": "00000000-0000-0000-0000-000000000000",
              "name": "string"
            },
            "id": "00000000-0000-0000-0000-000000000000",
            "description": "string",
            "url": "string",
            "mediaTypeId": "00000000-0000-0000-0000-000000000000",
            "order": 0
          }
        ],
        "dateToUnpin": "2018-11-19T13:01:25.197Z",
        "featuredColor": "string",
        "id": "00000000-0000-0000-0000-000000000000",
        "text": "string",
        "userId": "string",
        "datePosted": "2018-11-19T13:01:25.197Z",
        "userNamePosted": "string",
        "userPicture": "string",
        "liked": true,
        "likeCount": 0,
        "commentCount": 0
      }
    ]
  }
}
```