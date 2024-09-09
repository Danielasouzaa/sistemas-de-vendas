# Projeto 3: Sistema de Gerenciamento de Vendas

## Descrição

Este projeto implementa um sistema de banco de dados para gerenciar produtos, clientes e vendas em uma loja, utilizando SQL. O objetivo é criar um sistema eficiente para armazenar e manipular informações relacionadas a transações de vendas.

## Requisitos do Projeto

### Banco de Dados

1. **Nome do banco de dados**: `sistema_vendas`
2. **Tabelas**:
   - **Clientes**: Contém informações sobre os clientes, como:
     - `id_cliente` (INT, PK)
     - `nome` (VARCHAR)
     - `email` (VARCHAR)
     - `telefone` (VARCHAR)
   - **Produtos**: Contém informações sobre os produtos, como:
     - `id_produto` (INT, PK)
     - `nome_produto` (VARCHAR)
     - `preco` (DECIMAL)
     - `quantidade_estoque` (INT)
   - **Vendas**: Registra as vendas realizadas, como:
     - `id_venda` (INT, PK)
     - `id_cliente` (FK para `Clientes`)
     - `id_produto` (FK para `Produtos`)
     - `quantidade_vendida` (INT)
     - `data_venda` (DATE)

### Comandos Utilizados

- **CREATE DATABASE**: Para criar o banco de dados.
- **CREATE TABLE**: Para criar as tabelas de clientes, produtos e vendas.
- **INSERT INTO**: Para inserir dados nas tabelas.
- **SELECT JOIN**: Para consultar dados integrados das tabelas.
- **UPDATE**: Para atualizar o estoque de produtos e informações de clientes.
- **DELETE**: Para deletar vendas e, se necessário, clientes.

## Funcionalidades do Sistema

1. **Inserção de Dados**: Insira pelo menos 3 clientes, 3 produtos e 5 vendas.
2. **Consultas**:
   - Listar todas as vendas com o nome do cliente e produto.
   - Mostrar todas as compras de um cliente específico.
   - Exibir o total de vendas realizadas por produto.
3. **Atualizações**:
   - Atualizar o estoque de produtos após uma venda.
   - Atualizar as informações de um cliente.
4. **Deleções**:
   - Deletar uma venda e, opcionalmente, deletar o cliente associado.

## Como Executar

1. **Clonar o repositório**:
   ```bash
   git clone https://github.com/seu-usuario/sistema-vendas.git
   
Você pode personalizar o conteúdo do `README.md` conforme necessário e ajustar o `.gitignore` para incluir quaisquer outros arquivos específicos do seu ambiente de desenvolvimento.

