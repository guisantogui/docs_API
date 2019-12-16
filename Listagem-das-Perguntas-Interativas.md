## Assinatura do Endpoint

GET - cms/interactives/

## Descrição do negócio
Endpoint lista todas entidades do backend, respeitando os filtros e ordenado por:

1. Evento - propriedade Title na lingua portuguesa
2. Grupo - propriedade Name do grupo de interativa vinculado
3. Pergunta - propriedade Question

## Parametros na URL

####Parametros em via query
- question - filtra a interativa pelo sua pergunta
- grupo - filtra a interativa pelo nome do seu grupo
- carouselId - filtra interativas vinculados no carousel selecionado, ou nenhum
- eventId - filtra interativas vinculados no evento selecionado, ou nenhum
- hasGroup - filtra interativas sem vinculo com grupo, com vinculo, ou ambos
- [Parâmetros de paginação](/API-\(Endpoints\)/Parâmetros-de-paginação)

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": [
    {
      "id": "444444444-888888888-9999999",
      "question": "interativa",
      "time": 40,
      "type": "Titulo",
      "carousel": "descrição",
      "event": "SBC", //pegar o titulo PT-br
      "answersNumber": 51 //count das respostas para essa pergunta
    },
    {
      "id": "444444444-888888888-9999999",
      "question": "interativa",
      "time": 40,
      "type": "Titulo",
      "carousel": "descrição",
      "event": "SBC", //pegar o titulo PT-br
      "answersNumber": 51 //count das respostas para essa pergunta
    }
  ]
}
```