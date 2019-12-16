## Assinatura do Endpoint
GET - events/{id}/sponsors/{sponsorId}
GET - sponsors/{id} (NOVO, manter antigo)

## Descrição do negócio
Endpoint que busca todas informações do patrocinador.
O endpoint antigo deverá considerar sponsors ligados diretamente ao evento, ou ligados indiretamente via item no carousel.

## Parametros na URL
####GET - events/{id}/sponsors/{sponsorId}
- id - identificador do evento
- sponsorId - Identificador do sponsor

####GET - sponsors/{id}
- id - identificador do sponsor


##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": {
    "id": "00000000-0000-0000-0000-000000000000",
    "name": "string",
    "presentation": "string",
    "sponsorLevel": "string",
    "facebookLink": "string",
    "twitterLink": "string",
    "googlePlusLink": "string",
    "instagramLink": "string",
    "linkedinLink": "string",
    "genericLink": "string",
    "bannerPictureUrl": "string",
    "bannerDetailPictureUrl": "string"
  }
}
```