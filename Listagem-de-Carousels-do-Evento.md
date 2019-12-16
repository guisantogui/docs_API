
## Assinatura do Endpoint

GET - events/{id}/carousels

## Descrição do negócio
Endpoint que lista os itens de carousel que são exibidos acima da timeline do evento, que são dos possíveis tipos:
- Palestra
- Palestrante
- Patrocinador
- Conteúdo
- Interativa
- Link Simples
- Sem link

De acordo com a nova estrutura de grupos de carousel, poderemos ter um comportamento diferente, seguem as regras novas:
- Os itens de carousel poderão pertencer à um grupo ou pertencer diretamente à um evento/entidade, e então esse grupo pertencer à um evento. (Hoje o grupo não pertence a uma entidade)
- É possível ainda que um evento tenha um grupo de carousel vinculado e itens vinculados, os itens vinculados diretamente serão os primeiros itens listados, depois serão listados os itens do grupo.
- A regra de ordenação de itens ligados diretamente ao evento será:
  1. Campo Order ASC
  2. Campo StartVisibility DESC
- A regra de ordenação dos itens do grupo será a mesma dos itens ligados diretamente, porém para àquele grupo.
- O grupo de carousel também tem data de Start e fim, e os itens vinculados a ele, somente deverão ser visíveis quando a data atual estiver dentro do período.
- No grupo de carousels há um comportamento especial, há um campo CycleTime que é um inteiro não nulo, ele servirá para fazer o funcionamento da regra:
  - O objetivo é fazer que os itens dentro do grupo fiquem rodando à medida que o tempo passa, como uma lista sem fim, onde o último item da fila se tornará o primeiro com o passar do tempo definido, o primeiro item, se tornará o segundo e assim por diante.

PS: Tecnicamente pensei em sempre que o endpoint for chamado o "rodador" de itens verificaria se os itens estão ordenados de acordo, e caso sim retornariam, caso não ajustariam e depois retornariam, da pra fazer isso jogando com a Start/End Visibility do item do carousel, para não ter que criar um serviço pra monitorar isso.



## Descrição técnica
O id do evento deverá ser vinculado em uma tabela de ligação N para N, bem como a tabela de ligação entre Institution(Entidade) e Item de Carousel.

## Parametros na URL
id - Identificador do evento

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": [
    {
      "id": "00000000-0000-0000-0000-000000000000",
      "thumbnail": "string",
      "externalLink": "string",
      "exclude": true,
      "medias": [
        {
          "id": "00000000-0000-0000-0000-000000000000",
          "description": "string",
          "url": "string",
          "thumbnailUrl": "string",
          "dateCreated": "2018-11-19T13:01:25.286Z",
          "videoLength": "string",
          "mediaType": {
            "id": "00000000-0000-0000-0000-000000000000",
            "name": "string"
          },
          "featured": true,
          "order": 0,
          "speaker": {
            "id": "00000000-0000-0000-0000-000000000000",
            "name": "string"
          },
          "children": [
            {}
          ],
          "favorited": true
        }
      ],
      "talk": {
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
        "startDate": "2018-11-19T13:01:25.286Z",
        "endDate": "2018-11-19T13:01:25.286Z",
        "room": "string",
        "category": "string",
        "featuredColor": "string"
      },
      "interactiveGroup": {
        "id": "00000000-0000-0000-0000-000000000000",
        "name": "string",
        "place": "string",
        "startDate": "2018-11-19T13:01:25.286Z",
        "endDate": "2018-11-19T13:01:25.286Z",
        "labelDate": "string",
        "interactive": {
          "id": "00000000-0000-0000-0000-000000000000",
          "question": "string",
          "startDate": "2018-11-19T13:01:25.286Z",
          "endDate": "2018-11-19T13:01:25.286Z",
          "order": 0,
          "time": 0,
          "interactiveTypeId": "00000000-0000-0000-0000-000000000000",
          "answersOptions": [
            {
              "id": "00000000-0000-0000-0000-000000000000",
              "order": 0,
              "description": "string",
              "isRight": true
            }
          ]
        }
      },
      "speaker": {
        "id": "00000000-0000-0000-0000-000000000000",
        "name": "string"
      },
      "sponsor": {
        "id": "00000000-0000-0000-0000-000000000000",
        "name": "string"
      }
      "type": 1
    }
  ]
}
```
