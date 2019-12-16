## Assinatura do Endpoint

GET - cms/posts/{id}

## Descrição do negócio
Endpoint retorna as informações da postagem enviada por parametro.
Quando a postagem estiver em um paper ou talk a informação da entidade e do evento também deverão serem preenchidas afinal talks e papers sempre estarão atrelados à um evento ou entidade.
Os objetos a qual a postagem não pertencem deverão vir com valor nulo.

## Parametros na URL
id - identificador da postagem

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": {
    "id": "55454564654-5465484564-54464534",
    "text": "postagem",
    "user": {
      "email": "joao@makadu.net",
      "name": "João",
      "id": "55454564654-5465484564-54464534"
    },
    "event": {
      "id": "55555-99988552145-63555455",
      "title": "titulo"
    },
    "institution": {
      "id": "55555-99988552145-63555455",
      "name": "titulo"
    },
    "talk": {
      "id": "55555-99988552145-63555455",
      "title": "titulo"
    },
    "paper": {
      "id": "55555-99988552145-63555455",
      "title": "titulo"
    },
    "featuredColor": "#558844",
    "imageUrl": "http://image.com/png.png",
    "schedule": "03/12/2019 15:00:10",
    "pinDate": "03/12/2019 15:00:10",
    "unPinDate": "03/12/2019 15:00:10"
  }
}
```