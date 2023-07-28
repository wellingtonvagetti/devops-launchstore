# Projeto devops-launchstore

<h1 align="center">
  <img src="docker/.github/logo.png" alt="Launchstore" >
</h1>

## Tópicos 

[Sobre a Launchstore](#sobre-a-launchstore)

[Funcionalidades](#funcionalidades)

[Tecnologias e Ferramentas](#tecnologias-e-ferramentas)

[Instalação e uso](#instalação-e-uso)

[Licença](#licença)

<br>

## Sobre a Launchstore

Launchstore é um projeto de e-commerce, desenvolvido durante o bootcamp LaunchBase da [Rocketseat](https://rocketseat.com.br/), onde foram abordados conceitos como MVC, controle de sessões, criptografia de senhas, envio de e-mails, upload de imagens, validações no back e front end, animações, dentre outros.

<h3 align="center">Home</h3>
<p align="center">
  <img src="docker/.github/home.png" alt="página principal">
</p>

<br>

<h3 align="center">Carrinho de Compras</h3>
<p align="center">
  <img src="docker/.github/cart.png" alt="carrinho de compras">
</p>

<br>

<h3 align="center">Pesquisa de Produtos</h3>
<p align="center">
  <img src="docker/.github/search.png" alt="pesquisa de produtos">
</p>

<br>

<h3 align="center">Página de Produto</h3>
<p align="center">
  <img src="docker/.github/product.png" alt="página de produto">
</p>

<br>

## Funcionalidades

- [X] Cadastro de usuários.
- [X] Criação de anúncios.
- [X] Realização de pedidos.
- [X] Carrinho de compras.
- [X] Buscar produtos.
- [X] Upload de imagems com Multer.
- [X] Páginas dinâmicas com Nunjucks.
- [X] Banco de dados PostgreSQL.
- [X] Sistema de login e recuperação de senha.
- [X] Animações com Lottie.

<br>

## Tecnologias e Ferramentas

As seguintes tecnologias foram utilizadas no desenvolvimento do projeto:

- [HTML](https://devdocs.io/html/)
- [CSS](https://devdocs.io/css/)
- [JavaScript](https://devdocs.io/javascript/)
- [Nunjucks](https://mozilla.github.io/nunjucks/)
- [NodeJS](https://nodejs.org/en/)
- [Nodemailer](https://nodemailer.com/about/)
- [Express](https://expressjs.com/)
- [Express Session](https://github.com/expressjs/session)
- [Multer](https://github.com/expressjs/multer)
- [PostgreSQL](https://www.postgresql.org/)
- [BcryptJS](https://github.com/dcodeIO/bcrypt.js)
- [Faker.js](https://github.com/Marak/Faker.js)
- [Lottie](https://airbnb.design/lottie/)

<br>

## Instalação e Uso

Para rodar a aplicação, você precisa instalar o [Node](https://nodejs.org/en/) e o banco de dados [Postgres](https://www.postgresql.org/).

Siga os passos abaixo:

```bash
# Abra um terminal e copie este repositório com o comando
$ git clone https://github.com/martins-rafael/launchstore.git
# ou use a opção de download.

# Entre na pasta com 
$ cd launchstore

# Instale as dependências
$ npm install

# Crie o banco de dados e as tabelas utilizando os comandos
$ docker run --name postgres -e POSTGRES_PASSWORD=password -p 5432:5432 -d postgres
# inclusos no arquivo "database.sql".
    
# Conexão com o banco de dados:
# Abra e edite o arquivo "db.js" dentro da pasta "src/config"
# com o seu user e password do Postgres.

# Popule o banco de dados usando o aquivo "seed.js":
$ node seed.js

# Rode a aplicação
$ npm start
```

**Importante:** Cuidado ao alterar/excluir a imagem de placeholder da pasta `plublic/images`, pois os produtos gerados pelo `seed.js` compartilham esse arquivo entre si.

<br>

## Licença
<a href="https://opensource.org/licenses/MIT">
    <img alt="License" src="https://img.shields.io/badge/license-MIT-04cc5e?style=flat-square">
</a>

<br>

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](/LICENSE) para mais detalhes.
