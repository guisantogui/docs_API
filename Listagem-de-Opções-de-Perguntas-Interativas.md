## Assinatura do Endpoint

GET - cms/interactiveOptions/

## Descrição do negócio
Endpoint lista todas entidades do backend, respeitando os filtros e ordenado por:

1. Evento - propriedade Title na lingua portuguesa
2. Grupo - propriedade Name do grupo de interativa vinculado
3. Pergunta - propriedade Question da pergunta interativa

## Parametros na URL

####Parametros em via query
- answerOption - filtra pela descrição da opção
- interactiveQuestion - filtra as opções pela sua pergunta
- interactiveGroup - filtra as opções pelo nome dos grupos de interativa
- hasQuestion - filtra as opções com vinculo à uma pergunta, sem vinculo, ou ambas
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
      "answerOption": "opção",
      "order": 4,
      "interactiveQuestion": "Pergunta",
      "interactiveGroup": "Grupo",
      "isRight": true,
      "event": "SBC", // Titulo PT do evento
      "carousel": "",
      "selectedTimes": 12 // quantidade de vezes que algum usuário votou nessa opção
    },
    {
      "id": "444444444-888888888-9999999",
      "answerOption": "opção",
      "order": 4,
      "interactiveQuestion": "Pergunta",
      "interactiveGroup": "Grupo",
      "isRight": true,
      "event": "SBC", // Titulo PT do evento
      "carousel": "",
      "selectedTimes": 12 // quantidade de vezes que algum usuário votou nessa opção
    }
  ]
}
```