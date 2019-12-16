##Parametros enviados na query string

O CMS fará requisições de GET ao backend para consultar informações. Os filtros das buscas serão enviados na _queryString_ da URL, todo filtro que não for preenchido pelo usuário não deverá ser enviado ao backend na _queryString_, sendo assim, somente os filtros utilizados pelo usuário serão enviados.

##Listagem de Headers utilizados nos endpoints

##Obrigatórios
Os endpoints obrigatórios precisam ser preenchidos nas chamadas à API.

 - Header informando a versão da API utilizada
 - Header informando o token de autenticação
   - Este token será o Id do usuário, e a API deverá validar se o usuário tem a "role: CMSAdmin"
 - Header informando da onde as requisições estão indo, com o valor fixo "cms"

##Opcionais
Os endpoints opcionais não precisam ser preenchidos nas chamadas à API, porém é importante lembrar que as algumas funcionalidades precisam do preenchimento deles.

 - Header de plataforma que está acessando (ios, android, web)
 - Header enviando o idioma

PS: Não será obrigatório o envio do header M_whitelabel, nas requisições do CMS.