## Assinatura do Endpoint

GET - cms/papers/

## Descrição do negócio
Endpoint responsável por buscar todos papers do banco de dados, o endpoint deverá respeitar os filtros descritos.
OBS: Não há ordenação especificada.

## Parametros na URL
Não há

####Parametros em via query
- author - texto buscar por contains na tabela de ligação Author
- title - texto buscar por contains na tabela de ligação PaperLanguage
- uniqueId - texto buscar por contains na tabela Paper
- event - texto buscar por contains na tabela de ligação Event/EventLanguage
- category - texto buscar por contains na tabela de ligação PaperLanguage
- place - texto buscar por contains na tabela de ligação PaperLanguage
- institution - texto buscar por contains na tabela de ligação PaperLanguage
- hasSets - filtra papers com sets vinculados, sem sets vinculados, ou ambos
- hasCompletedEvaluation - **filtro complexo**, deve verificar dentre todos avaliadores vinculados se todos fizeram avaliação, somente deve retornar true, caso todos eles tenham realizado a avaliação
- hasMedia - filtra papers com mídia, sem mídia, ou ambos
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
      "id": "000987890=937895-486384-8737383",
      "title": "titulo da langauge PT",
      "uniqueId": "98-09",
      "event": "titulo da langauge PT do evento vinculado",
      "institution": "Coluna institutionName (Nova)",
      "category": "category da language PT",
      "hasSets": true,
      "EvaluationCompleted": false,
      "hasEvaluators": false,
      "hasMedia": true
    },
    {
      "id": "000987890=937895-486384-8737383",
      "title": "titulo da langauge PT",
      "uniqueId": "98-09",
      "event": "titulo da langauge PT do evento vinculado",
      "institution": "Coluna institutionName (Nova)",
      "category": "category da language PT",
      "hasSets": true,
      "EvaluationCompleted": false,
      "hasEvaluators": false,
      "hasMedia": true
    }
  ]
}
```