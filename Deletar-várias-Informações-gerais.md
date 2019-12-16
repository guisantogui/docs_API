## Assinatura do Endpoint

POST - cms/generalInfo/deleteBatch

## Descrição do negócio
Endpoint que receberá vários Id's de informação geral e deverá deletar todas do banco de dados, bem como seus vinculos com evento e entidade.

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
```
{
  "generalInfos": ["080808080845-16454654-4561-454454545", "080808080845-16454654-4561-454454545",
                   "080808080845-16454654-4561-454454545"]
}
```

##Objeto de retorno

```
{
  "response": true
}
```