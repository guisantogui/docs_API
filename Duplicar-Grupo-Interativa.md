## Assinatura do Endpoint

POST - cms/interactiveGroups/duplicate/{id}

## Descrição do negócio
Endpoint responsável duplicar um grupo de interativas por completo.
Regras:
 - O nome do grupo deverá ter o texto "Duplicado" no início.
 - Vinculo (deverá ser mantido o mesmo vinculo da interativa duplicada, no evento ou carousel)

Sendo assim os itens que deverá ser duplicados da interativa:
- Todas as Perguntas Interativas vinculadas à ele;
- Todas as Opções de todas Perguntas interativas;

OBS: As respostas não deverão ser duplicadas caso existam.

## Parametros na URL
id - Identificador do grupo de pergunta interativa

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