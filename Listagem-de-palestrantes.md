## Assinatura do Endpoint

GET - cms/speakers/

## Descrição do negócio
Endpoint lista todas entidades do backend, respeitando os filtros e ordenado por:
1. Name

A busca devera respeitar as seguintes regras na busca:

- Talk
   - Caso o speaker não esteja vinculado a nenhuma talk, o campo deverá vir uma string vazia
   - Caso o speaker esteja vinculado a apenas uma talk, deverá trazer o "Title" em português dela
   - Caso o speaker esteja vinculado a mais de uma talk, deverá trazer o texto "+ de 1"

- Evento
   - Caso o speaker não esteja vinculado a nenhum evento (através da talk), o campo deverá vir uma string vazia
   - Caso o speaker esteja vinculado a apenas um evento (através da talk), deverá trazer o "Title" em português dela
   - Caso o speaker esteja vinculado a mais de um evento (através da talk), deverá trazer o texto "+ de 1"


## Parametros na URL

####Parametros em via query
- name - filtra palestrante pelo seu nome
- talk - filtra somente palestrantes da talk descrita, filtro deve ser no campo title da tabela de traduções
- event - filtra somente palestrantes do evento descrita, filtro deve ser no campo title da tabela de traduções
- hasPicture - filtra palestrantes com foto, sem foto, ou ambos
- hasResume -  filtra palestrantes com curriculo, sem curriculo, ou ambos
- [Parâmetros de paginação](/API-\(Endpoints\)/Parâmetros-de-paginação)

OBS: Envio de booleanos que podem ser "ambos" com base nos [Parâmetros para consultas com boolean](/API-\(Endpoints\)/Parâmetros-para-consultas-com-boolean)

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
      "title": "João das Couves",
      "talk": "title OU + de 1", // registro em português
      "event": "title OU + de 1", // registro em português
      "about": "Primeiros 50 caracteres", // registro em português
      "photoLink": "http://www.makaduapi.com/photo2.jpg"
    },
    {
      "id": "55454564654-5465484564-54464534",
      "name": "Suelen Kristina",
      "talk": "title OU + de 1", // registro em português
      "event": "title OU + de 1", // registro em português
      "about": "Primeiros 50 caracteres", // registro em português
      "photoLink": "http://www.makaduapi.com/photo5.jpg"
    }
    ]
}
```