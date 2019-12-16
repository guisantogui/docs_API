## Assinatura do Endpoint

PUT - posts/{postId}

## Descrição do negócio
Endpoint que edita a postagem do evento.

## Parametros na URL
postId - identificador da postagem

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