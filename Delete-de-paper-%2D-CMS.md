## Assinatura do Endpoint

DELETE - cms/papers/{id}

## Descrição do negócio
Endpoint responsável por buscar os deletar um paper, fisicamente.
- Caso o paper tenha mídia vinculada, deverá ser deletada em cascade.
- Caso o paper tenha postagens vinculadas, deverão serem deletas em cascade, levando, likes, comentários, e comentários de likes (talvez usar a mesma função do delete de postagem seja inteligente)
- Caso o paper seja esteja curtido por algum usuário, as curtidas deverão serem removidas, não há cascade nesse caso.
- Caso o paper tenha sido trazido via integração, deverá deletar seu vinculo com a integração, não há cascade nesse caso.
- Caso o paper esteja vinculado em um ou mais sets de avaliação, deverá deletar seus vínculos, não há cascade nesse caso.
- Caso o paper esteja vinculado na tabela de userPaperEvaluator deverá deletar seus vinculos, removendo em cascade os regristros vinculados.


## Parametros na URL
- id - Identificador do id do paper

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