# WebServiceSpringBootJPA-Hibernate-Heroku

## Sobre o projeto

Esse projeto consiste em uma aplicação Java back-end, o qual foi inspirado no modelo relacional abaixo, sendo possível nesta aplicação fazer o CRUD de um usuário, e conseguir visualizar os produtos, categorias , e pedidos que estão cadastrados no banco. Para fazer todas essas operações da aplicação, será explicado mais abaixo quais são seus respectivos endpoints.

![ModeloRelacionalDB](https://user-images.githubusercontent.com/54071089/78404310-8437fe00-75d4-11ea-8065-023904c435c9.png)

### Tecnologias

Foram utilizadas diversas tecnologias interessantes para o desenvolvimento dessa aplicação, sendo uma delas o Hibernate, o qual é responsável pelo mapeamento objeto-relacional, facilitando muito no processo de criação do banco de dados. Outra ferramenta que auxilia muito é o banco de dados em memória H2, que nos facilita e nos permite uma rápida resposta de como o banco está no seu estado atual.

Para a versão de produção do projeto, foi feito um deploy no heroku com o banco de dados PostgreSQL, onde agora a aplicação pode ser acessada de qualquer computador.


## Endpoints

Link para acesso da aplicação: https://course-javasb-dks.herokuapp.com/

Recomendo o uso do Postman, pois assim será possivel ver o código de Status HTTP, e facilitará nas consultas de "GET", pois virão no padrão "JSON".

###  User

* Criação de usuário:

| End Point | Method | Params | Sucess Response |
| ---------- | ----------|----------|-------------------|
| /users      | POST      |  | Code: 201- Created|

body:
{
	name:  '?'
	email:  '?'
	phone: '?'
	password: '?'
}

* Busca de todos usuários:

| End Point | Method | Params | Sucess Response |
| ---------- | ----------|----------|-------------------|
| /users      | GET        |              | Code: 200 - Ok   |

* Busca de  usuários por id:

| End Point | Method | Params | Sucess Response |
| ---------- | ----------|----------|-------------------|
| /users      | GET        |  id         | Code: 200 - Ok   |

* Atualização de usuários por id:

| End Point | Method | Params | Sucess Response |
| ---------- | ----------|----------|-------------------|
| /users      | PUT      |  id         | Code: 200 - Ok   |

body:
{
	name:  '?'
	email:  '?'
	phone: '?'
}

* Deleção de usuário por id:

| End Point | Method | Params | Sucess Response |
| ---------- | ----------|----------|-------------------|
| /users      | DELETE   |  id         | Code: 204 - No Content|

### Produto

* Busca de todos os produtos:

| End Point | Method | Params | Sucess Response |
| ---------- | ----------|----------|-------------------|
| /products | GET        |              | Code: 200 - Ok   |

* Busca de produto por id:

| End Point | Method | Params | Sucess Response |
| ---------- | ----------|----------|-------------------|
| /products | GET       |  id         | Code: 200 - Ok   |

### Pedido

* Busca de todos os pedidos:

| End Point | Method | Params | Sucess Response |
| ---------- | ----------|----------|-------------------|
| /orders    | GET        |              | Code: 200 - Ok   |

* Busca de produto por id:

| End Point | Method | Params | Sucess Response |
| ---------- | ----------|----------|-------------------|
| /products | GET       | id          | Code: 200 - Ok   |

### Categoria

* Busca de todas as categorias:

| End Point | Method | Params | Sucess Response |
| ---------- | ----------|----------|-------------------|
| /products | GET        |              | Code: 200 - Ok   |

* Busca de categoria por id:

| End Point | Method | Params | Sucess Response |
| ---------- | ----------|----------|-------------------|
| /products | GET       |id            | Code: 200 - Ok   |

## Agradecimentos e contatos
Agora, é só testar a aplicação! Todo e qualquer feedback é incentivado e muito apreciado. Qualquer dúvida pode ser enviada para douglasks99@gmail.com. Obrigado pelo interesse!
