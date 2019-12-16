## Assinatura do Endpoint

GET - cms/sponsors/

## Descrição do negócio
Endpoint lista todas entidades do backend, respeitando os filtros e ordenado por:
1. Evento (TitlePT)
2. Order

## Parametros na URL

####Parametros em via query
- name - filtra itens pela descrição
- event - filtra itens pelo titulo PT do evento
- institution - filtra itens pelo nome PT do evento
- [Parâmetros de paginação](/API-\(Endpoints\)/Parâmetros-de-paginação)

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": [
    {
      "id": "55454564654-5465484564-54464534",
      "name": "item X",
      "event": "evt OU + de 1",
      "institution: "inst 1 ou + de 1",
      "thumbnail": "http://www.makaduapi.com/photo2.jpg",
      "presentation": "apresentação",
      "order": 1,
      "sponsorLevel": "platinum ou + de 1"
    },
    {
      "id": "55454564654-5465484564-54464534",
      "name": "item X",
      "event": "evt2 ou + de 1",
      "institution: "inst 1 ou + de 1",
      "thumbnail": "http://www.makaduapi.com/photo2.jpg",
      "presentation": "apresentação",
      "order": 1,
      "sponsorLevel": "ouro ou + de 1"
    }
    ]
}
```