## Assinatura do Endpoint

GET - cms/whitelabel/

## Descrição do negócio
Retorna as informações dos white labels presentes no backend, ordenado por:
1. Titulo ASC
2. Possui vinculo com entidade (As que possuem acima)

## Parametros na URL
Não há

####Parametros em query
- title - filtra os white labels pelo nome, "modo contains"
- hasEntity - filtra todos whitelabels que tem vinculo com alguma Institution(Entidade), se for true, é obrigatório ter o vínculo, se for false, é obrigatório não ter o vínculo
- [Parâmetros de paginação](/API-\(Endpoints\)/Parâmetros-de-paginação)

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": 
  [
    {
      "id": "0000000-0000000-000000000",
      "title": "Makadu",
      "typeId": 1,
      "linkIOS: "",
      "linkAndroid":"",
      "institution": {
        "id": "000000-0000000-000000000",
        "title": "Titulo",
        "timelineType": 1
      } // ou null
    } 
    ,
    {
      "id": "0000000-0000000-000000000",
      "title": "Makadu",
      "typeId": 1,
      "linkIOS: "",
      "linkAndroid":"",
      "institution": {
        "id": "000000-0000000-000000000",
        "title": "Title",
        "timelineType": 2
      } // ou null
    }
  ]
}
```