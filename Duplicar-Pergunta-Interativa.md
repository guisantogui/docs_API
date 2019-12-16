## Assinatura do Endpoint

POST - cms/interactives/duplicate/{id}

## Descrição do negócio
Endpoint responsável duplicar uma interativa por completo.
Regras:
 - A pergunta deverá ter o texto "Duplicado" no início.
 - Vinculo (deverá ser mantido o mesmo vinculo da interativa duplicada no grupo de interativa)

Sendo assim os itens que deverá ser duplicados da interativa:
- Todas as Opções de todas Perguntas interativas;

OBS: As respostas não deverão ser duplicadas caso existam.

## Parametros na URL
id - Identificador da pergunta interativa

##Parametros em cabeçalho
[Parametros padrão CMS](/API-\(Endpoints\)/Parametros-padrão-CMS)

##Objeto de envio
Não se aplica

##Objeto de retorno

```
{
  "response": true
}
```