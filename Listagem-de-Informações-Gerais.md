## Assinatura do Endpoint

GET - cms/generalInfo/

## Descrição do negócio
Endpoint lista todas entidades (GeneralInfo) do backend, respeitando os filtros e ordenado por:
1. Evento (TitlePT)
2. Order

## Parametros na URL

####Parametros em via query
- title - filtra itens pelo seu título, filtro deve ser no campo da tabela de traduções
- description - filtra itens pela sua descrição, filtro deve ser no campo da tabela de traduções
- event - filtra somente itens do evento descrito, filtro deve ser no campo title da tabela de traduções
- institution - filtra somente itens da institution descrita, filtro deve ser no campo name da tabela de traduções
- active - filtra itens ativos, ou inativos, ou todos (caso não envie o parâmetro)
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
      "title": "item X",
      "type": "FAQ/Aviso/MAPA/Regulamento",
      "event": "evt OU (+ de 1)",
      "formatAsHTML": true,
      "active": true,
      "order": 1
    },
    {
      "id": "55454564654-5465484564-54464534",
      "title": "item X",
      "type": "FAQ/Aviso/MAPA/Regulamento",
      "event": "evt OU (+ de 1)",
      "formatAsHTML": true,
      "active": true,
      "order": 1
    }
    ]
}
```