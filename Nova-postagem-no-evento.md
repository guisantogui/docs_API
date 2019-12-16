## Assinatura do Endpoint

POST - /events/{id}/posts

## Descrição do negócio
Cria uma nova postagem no evento

## Parametros na URL
id - identificador do evento

##Parametros em cabeçalho
[Parâmetros Padrão](/API-\(Endpoints\)/Parâmetros-Padrão)

- Arquivo binário: Imagem da postagem, enviado como Multipart header
- Json: Texto da postagem, enviada string com encoding = "x-www-form-urlencoded" no formato json abaixo:

```
{
    "text": ""
}
```


##Objeto de envio
Não se aplica


##Objeto de retorno

```
{
  "response": true
}
```