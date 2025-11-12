# Sistema Simplificado de Gerenciamento de Tarefas

Projeto em Node.js + Express desenvolvido por **Leandro Bragaça da Silva** para praticar CRUD e programação assíncrona (armazenamento em memória).

## Objetivo
Este projeto tem como objetivo consolidar o entendimento sobre **programação assíncrona** em Node.js, utilizando **Promises**, **async/await** e **callbacks**, aplicados em um sistema simples de gerenciamento de tarefas.

## Requisitos
- Node.js v14+ (recomendado v16+)

## Instalação

1. Clone ou baixe os arquivos deste repositório.
2. No diretório do projeto, execute o comando:

```bash
npm install
```

3. Para iniciar o servidor, execute:

```bash
npm start
```

Ou em modo de desenvolvimento (com nodemon):

```bash
npm run dev
```

O servidor rodará em `http://localhost:3000` por padrão.

## Rotas Disponíveis

### Listar tarefas
`GET /tasks`

Retorna todas as tarefas cadastradas.

### Criar tarefa
`POST /tasks`

Cria uma nova tarefa.

**Exemplo de body JSON:**
```json
{
  "titulo": "Estudar Node.js",
  "status": "pendente"
}
```

### Atualizar tarefa
`PUT /tasks/:id`

Atualiza uma tarefa existente.

**Exemplo de body JSON:**
```json
{
  "status": "concluída"
}
```

### Deletar tarefa
`DELETE /tasks/:id`

Remove uma tarefa pelo ID.

## Observações
- As tarefas são armazenadas em **memória**, ou seja, os dados são apagados quando o servidor é reiniciado.
- O código foi estruturado para fácil migração futura para um banco de dados real.

## Autor
**Leandro Bragaça da Silva**  
Projeto desenvolvido como parte prática de estudo em **Node.js e Express**.

---
📅 *Última atualização: Novembro de 2025*
