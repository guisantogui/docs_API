## Assinatura do Endpoint

GET - cms/posts/

## Descrição do negócio
Endpoint lista todas postagens do backend. Respeitando filtros e ordenação:
Ordenação:
1. DateCreate - DESC (Mais novo para mais velho)

## Parametros na URL

####Parametros em via query
- text - filtra a postagem pelo seu conteúdo
- evento - filtra pela propriedade title do evento
- entidade - filtra pela propriedade name da entidade
- email - filtra pelo email do usuário dono da postagem
- postagens verificadas - filtra postagens de todos usuários, ou apenas verificados
- titulo da talk - filtra postagens pelo título da talk
- titulo do paper - filtra postagens pelo título do paper
- tipo de timeline
  - TODOS
  - 1 (Evento)
  - 2 (Institution)
  - 3 (Talk)
  - 4 (Paper)
- Ativo - Filtra postagens ativas, inativas, ou ambas
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
      "text": "postagem",
      "emailUserOwner":"joao@makadu.net",
      "verifiedUser": true,
      "timeline": "AQUI pode ser o titulo do evento/talk/entidade/paper",
      "scheduled": "03/12/2019 15:00:10"
    },
    {
      "id": "55454564654-5465484564-54464534",
      "text": "postagem",
      "emailUserOwner":"joao@makadu.net",
      "verifiedUser": true,
      "timeline": "AQUI pode ser o titulo do evento/talk/entidade/paper",
      "scheduled": "03/12/2019 15:00:10"
    }
    ]
}
```