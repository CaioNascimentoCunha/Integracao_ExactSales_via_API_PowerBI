# Integr_ExactSales_PowerBI
Nesse projeto, irei ajudar aos usuários do CRM da Exact Sales - o Spotter - a superar a limitação de requisições via API que o sistema disponibiliza.

Para quem não conhece Spotter  é um software de sales engagement voltado para equipes de venda Inside Sales, que te ajuda a converter mais leads em vendas. E ele faz isso coletando dados que vão enriquecer a qualificação de leads em oportunidades. Por isso, extrair estas informações e combiná-las com outras fontes irá melhorar muito suas análises.

Como gestor da área me deparei com o desafio de aprofundar nossas analises para trazer inteligencia comercial para o time e por isso resolvi conectar os dados extraídos do sistema para um dashboard em Power BI que permitisse trazer novas analises.

Porém a API do Spotter é do tipo REST e usa o protocolo OData. Outro detalhe importante é que ela é paginada, e retorna no máximo 500 registros por requisição. Uma API REST permite que você faça requisições do tipo GET para conseguir os dados que estão armazenados no banco de dados do software. E o protocolo OData permite que você aplique consultas similares ao SQL como parâmetro da requisição. Se você só quer dados de uma determinada data, ou quer só 2 colunas da tabela, isso é muito útil. Ainda assim, essas limitações impedem que se faça analises de longo prazo para usuários com bases extensas

A baixo vou compartilhar a solução que desenvolvi para ultrapassar as limitações de requisição e analisar toda a base de dados que possuir no Spotter

Documentações que podem ajudar:
https://exactsales.freshdesk.com/pt-BR/support/solutions/articles/73000614979-filtros-api
https://exactspotter.docs.apiary.io/#
https://exactsales.freshdesk.com/pt-BR/support/solutions/articles/73000614979-filtros-api
