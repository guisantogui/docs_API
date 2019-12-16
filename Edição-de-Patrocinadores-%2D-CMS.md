## Assinatura do Endpoint

PUT - cms/sponsor/

## Descrição do negócio
Endpoint que edita uma entidade (sponsor) e seus vinculos no banco de dados, removendo ou excluindo-os.

## Parametros na URL
Não há

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

Até 2 arquivos binários (Imagem da postagem, enviado como Multipart header)

- thumbnail
- mainImage

Json: Texto da postagem, enviada string com encoding = "x-www-form-urlencoded" no formato json abaixo:

```
{
  "id": "855852489648-5548858555-98988999",
  "name": "Patrocinador",
  "presentationPT": "",
  "presentationES": "",
  "presentationEN": "",
  "facebookLink": "",
  "linkedinLink": "",
  "twitterLink": "",
  "instagramkLink": "",
  "genericLink": "",
  "order": 2,
  "events": [
    {
      "id":"855852489648-5548858555-98988999",
      "sponsorLevel": "Prata"
    }
    , {
      "id":"855852489648-5548858555-98988999",
      "sponsorLevel": "Prata"
    }],
  "institutions": [{
      "id":"855852489648-5548858555-98988999",
      "sponsorLevel": "Prata"
    },
    {
      "id":"855852489648-5548858555-98988999",
      "sponsorLevel": "Prata"
    }],
    "removeThumbnail": false,
    "removeMainImage": false
}
```


##Objeto de envio
Não há

##Objeto de retorno

```
{
  "response": true
}
```