Sistema de Gerenciamento de Tarefas

Autor: Leandro Bragaça da Silva

Este projeto é um sistema simples de gerenciamento de tarefas desenvolvido em Node.js + Express, com armazenamento em um arquivo JSON. O objetivo é demonstrar a criação de rotas, controllers, estrutura MVC e manipulação de dados.

Tecnologias Utilizadas

Node.js

Express

File System (fs)

Nodemon

JavaScript

Estrutura do Projeto
Task-manager/
│── controllers/
│     └── taskController.js
│── routes/
│     └── taskRoutes.js
│── data/
│     └── tasks.json
│── index.js
│── package.json
│── README.md

Como Rodar o Projeto
1. Instale as dependências
npm install

2. Inicie o servidor
node index.js


Se tudo estiver correto, aparecerá:

Servidor rodando na porta 3000

Rotas Disponíveis
Listar todas as tarefas

GET /tasks

Criar nova tarefa

POST /tasks
Body JSON:

{
  "title": "Título da tarefa",
  "description": "Descrição da tarefa"
}

Buscar tarefa pelo ID

GET /tasks/:id

Atualizar tarefa

PUT /tasks/:id

Deletar tarefa

DELETE /tasks/:id

Objetivo do Projeto

Este sistema foi desenvolvido como parte do estudo de:

Estrutura MVC

CRUD básico

Manipulação de JSON

Criação de API com Express

Autor

Leandro Bragaça da Silva
