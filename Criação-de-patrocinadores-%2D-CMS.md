## Assinatura do Endpoint

POST - cms/sponsor/

## Descrição do negócio
Endpoint que cria uma nova entidade (sponsor), e retorna se a criação foi feita com sucesso.

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
    }]
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