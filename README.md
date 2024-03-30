# Projeto de Posts

Este é um projeto de uma aplicação de posts desenvolvida utilizando Express.js para criar uma API RESTful para manipulação de dados e WebSocket (Socket.io) para comunicação em tempo real. O front-end da aplicação não está incluso neste repositório, pois o foco é o backend e ele já foi utilizado pronto.

## Funcionalidades Principais

- **Autenticação**: O sistema possui um sistema de autenticação que permite aos usuários efetuarem login e cadastro, utilizando bcrypt para criptografar senhas e jsonwebtoken para geração e verificação de tokens.
- **Posts**: Os usuários autenticados podem criar, visualizar, atualizar e excluir posts.
- **Upload de Imagens**: Os usuários podem fazer upload de imagens para serem usadas nos posts.
- **Comunicação em Tempo Real**: Utiliza WebSocket (Socket.io) para permitir a comunicação em tempo real entre os usuários.

## Tecnologias Utilizadas

- **Express.js**: Utilizado para criar a API RESTful.
- **Socket.io**: Biblioteca para comunicação em tempo real.
- **Express Validator**: Utilizado para validação de dados na requisição.
- **Bcrypt**: Utilizado para criptografar senhas.
- **JSON Web Token (JWT)**: Utilizado para autenticação de usuários.
- **Multer**: Middleware Node.js para lidar com upload de arquivos.
- **Mongoose**: ODM (Object Data Modeling) para MongoDB, utilizado para modelar os dados da aplicação.
- **MongoDB**: Banco de dados utilizado para armazenar os dados da aplicação.

## Configuração do Ambiente

1. Certifique-se de ter o Node.js e o MongoDB instalados em sua máquina.
2. Clone este repositório: `git clone git clone https://github.com/MatheusStarkX/NodeJs-RestAPI-Posts.git`.
3. Navegue até o diretório do projeto: `cd NodeJs-RestAPI-Posts`.
4. Instale as dependências: `npm install`.
5. Configure as variáveis de ambiente necessárias (veja abaixo).
6. Inicie o servidor: `npm start`.

### Variáveis de Ambiente

Configurações das seguintes variáveis de ambiente para iniciar o servidor:

- **PORT**: A porta em que o servidor irá rodar (app.js).
- **MONGO_URI**: URI de conexão com o MongoDB (app.js).
- **JWT_SECRET**: Chave secreta para geração de tokens JWT (middleware/is-auth.js e controllers/auth.js).

## Autor

Este projeto foi desenvolvido por [Matheus Felipe](https://github.com/MatheusStarkX) baseado no curso [NodeJS - The Complete Guide (MVC, REST APIs, GraphQL, Deno)](https://www.udemy.com/course/nodejs-the-complete-guide/?couponCode=KEEPLEARNING) da Udemy.
