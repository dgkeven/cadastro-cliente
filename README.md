# Cadastro de Clientes

Este é um projeto simples de cadastro de clientes utilizando **Node.js**, **Express**, **Sequelize** e um banco de dados **SQLite**.

## Funcionalidades

- Cadastro de clientes com os seguintes campos:
  - Nome
  - Data de nascimento
  - Cidade
  - Telefone
- Armazenamento dos dados em um banco SQLite.
- Exibição de uma página inicial e de um formulário para adicionar clientes.
- Persistência de dados usando Sequelize.

---

## Tecnologias Utilizadas

- **Node.js**: Para criar o servidor.
- **Express**: Framework para gerenciar rotas e requisições HTTP.
- **Sequelize**: ORM para manipulação do banco de dados.
- **SQLite**: Banco de dados leve e integrado ao projeto.
- **Bootstrap**: Para estilização do formulário.

---

## Pré-requisitos

Certifique-se de ter instalado em sua máquina:

- **Node.js**: [Download Node.js](https://nodejs.org)
- **npm** (vem junto com o Node.js)

---

## Como Executar o Projeto

1. Clone este repositório em sua máquina local:

   ```bash
   git@github.com:dgkeven/cadastro-cliente.git
   ```

2. Instale as dependências do projeto:

   ```bash
   npm install
   ```

3. Execute o servidor:

   ```bash
   node index.js
   ```

4. Acesse o servidor no navegador:

   ```
   http://localhost:9443
   ```

---

## Estrutura do Projeto

- **index.js**: Arquivo principal do projeto. Contém as rotas e a lógica do servidor.
- **db.js**: Configuração do banco de dados SQLite.
- **models/cliente.js**: Modelo Sequelize para a tabela de clientes.
- **views/formCliente.html**: Formulário HTML para cadastro de clientes.

---

## Endpoints Disponíveis

- `GET /`: Exibe uma mensagem de boas-vindas.
- `GET /cadcliente`: Retorna o formulário de cadastro de clientes.
- `POST /addcliente`: Processa o envio do formulário e cadastra um cliente no banco.

---

## Observações

- O formato da data de nascimento deve ser **AAAA-MM-DD**.
- Certifique-se de que o arquivo `cliente.sqlite` foi gerado na raiz do projeto após a execução.

---

## Melhorias Futuras

- Adicionar validações nos campos do formulário.
- Criar uma página para listar todos os clientes cadastrados.
- Implementar edição e exclusão de clientes.
- Substituir o SQLite por um banco de dados mais robusto (ex.: MySQL ou PostgreSQL) caso necessário.

---

## Contribuindo

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e enviar pull requests.

---
