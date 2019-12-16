## Assinatura do Endpoint

GET - cms/users/

## Descrição do negócio
Endpoint lista todos Usuários do backend, respeitando os filtros e ordenado por:

- Name
- Email

## Parametros na URL

####Parametros em via query
- Name - filtra usuários pelo email usando "contains" como modo de filtro
- Email - filtra usuários pelo email usando "contains" como modo de filtro
- Active - filtra usuários ativos ou não
- Verified - filtra usuários Verificados ou não
- Evento - filtra usuários que tem vinculo direto ao evento (contains)
- WhiteLabel - filtra usuários vinculados (indiretamente, pelo evento) ao white label (contains)
- Avaliador - filtra usuários avaliadores ou não (contains)
- Paper - filtra usuários avaliadores daquele paper (contains)

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  
  "response": [{
    "id": "78787878-99999-51545454-222111-6622411",
    "name": "joão",
    "email": "joao@gmail.com",
    "ativo": true,
    "verified": false,
    "evaluator": false
  },
  {
    "id": "78787878-99999-51545454-222111-6622411",
    "name": "pedro",
    "email": "pedro@gmail.com",
    "ativo": true,
    "verified": true,
    "evaluator": true
  }
  ]   
}
```