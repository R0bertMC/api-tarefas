# API de Tarefas 📝

Este é um projeto de API para gerenciamento de tarefas, desenvolvido com **Node.js** e **Express**.

## 🚀 Pré-requisitos
- **Node.js** (versão 14 ou superior)
- **npm** (gerenciador de pacotes do Node.js)

## 📦 Instalação

1. Clone o repositório:
   ```bash
   git clone <URL_DO_REPOSITORIO>
   cd api-tarefas
   ```

2. Instale as dependências:
   ```bash
   npm install
   ```

## 🚀 Executando o servidor

Modo normal:
```bash
npm start
```

Modo de desenvolvimento (com nodemon):
```bash
npm run dev
```

O servidor será iniciado em: `http://localhost:3000`

## 🌍 Endpoints disponíveis:

### 1️⃣ Rota Inicial
- **Método:** `GET`
- **URL:** `/`
- **Descrição:** Testa se a API está funcionando.
- **Resposta:** `"API de tarefas funcionando!"`

### 2️⃣ Listar todas as tarefas
- **Método:** `GET`
- **URL:** `/tarefas`
- **Descrição:** Retorna todas as tarefas cadastradas.

### 3️⃣ Listar uma tarefa por ID
- **Método:** `GET`
- **URL:** `/tarefas/:id`
- **Descrição:** Retorna uma tarefa específica pelo ID.

### 4️⃣ Criar uma nova tarefa
- **Método:** `POST`
- **URL:** `/tarefas`
- **Descrição:** Cria uma nova tarefa.
- **Corpo da requisição (JSON):**
  ```json
  {
    "titulo": "Nova Tarefa",
    "descricao": "Descrição da nova tarefa",
    "concluida": false
  }
  ```

### 5️⃣ Atualizar uma tarefa por ID
- **Método:** `PUT`
- **URL:** `/tarefas/:id`
- **Descrição:** Atualiza uma tarefa específica pelo ID.
- **Corpo da requisição (JSON):**
  ```json
  {
    "titulo": "Tarefa Atualizada",
    "descricao": "Descrição atualizada",
    "concluida": true
  }
  ```

### 6️⃣ Marcar uma tarefa como concluída
- **Método:** `PATCH`
- **URL:** `/tarefas/:id/concluir`
- **Descrição:** Marca uma tarefa como concluída.

### 7️⃣ Deletar uma tarefa por ID
- **Método:** `DELETE`
- **URL:** `/tarefas/:id`
- **Descrição:** Remove uma tarefa específica pelo ID.

### 8️⃣ Rota inválida (404)
- **Descrição:** Qualquer rota não definida retornará:
  ```json
  {
    "mensagem": "Rota não encontrada."
  }
  ```

## ⚙️ Tecnologias utilizadas
- **Node.js**
- **Express**
- **Joi** (validação de dados)
- **UUID** (geração de IDs únicos)
- **Nodemon** (recarregamento automático no desenvolvimento)
=======
# api-tarefas
API para gerenciamento de tarefas com Node.js e Express.

