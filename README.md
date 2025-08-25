# 🛒 E-commerce Database Model

Este projeto consiste na modelagem e criação de um banco de dados relacional para um sistema de **e-commerce (loja virtual)**. Ele foi desenvolvido como parte do desafio prático do curso **"Randstad - Análise de Dados"** promovido pela **Digital Innovation One (DIO)**.

---

## 📌 Objetivo

Criar um esquema de banco de dados relacional completo e normalizado para gerenciar:

- Clientes (Pessoa Física e Jurídica)
- Pedidos e seus produtos
- Entregas
- Estoques
- Fornecedores
- Vendedores terceirizados
- Formas de pagamento

---

## 🧠 Modelo Conceitual

O projeto é baseado em um modelo conceitual que visa representar o funcionamento de uma loja virtual moderna, com diferentes tipos de clientes, múltiplos estoques, integração com fornecedores e controle de entregas. O banco permite acompanhar o ciclo completo de um pedido, desde sua criação até a entrega, com flexibilidade para formas de pagamento e gestão de estoque.

---

## 🛠️ Tecnologias Utilizadas

- **MySQL Workbench** – para modelagem e geração do script SQL
- **MySQL Server** – como sistema gerenciador de banco de dados
- **Workbench EER Diagram** – utilizado para criação do modelo ER
- **Git/GitHub** – versionamento e hospedagem do projeto

---

## 📂 Estrutura do Projeto

- `ecommerce-database.sql` – script de criação do banco de dados com todas as tabelas, chaves primárias e estrangeiras
- `ecommerce_model.png` – imagem do modelo conceitual
- `README.md` – documentação e contexto do projeto

---

## 🧩 Entidades principais

- `cliente`, `pessoa_fisica`, `pessoa_juridica`
- `pedido`, `pedido_produto`, `entrega`
- `produto`, `estoque`, `produto_estoque`
- `fornecedor`, `fornecedor_produto`
- `vendedor_terceiro`, `fk_vendedor_terceiro_produto`
- `forma_pagamento`, `forma_pagamento_cliente`

---

## 📈 Relacionamentos importantes

- Um cliente pode ter vários pedidos e várias formas de pagamento.
- Cada pedido pode conter vários produtos.
- Os produtos podem estar em vários estoques ou com diferentes vendedores.
- A entrega está associada a um pedido e possui transportadora, status e rastreamento.

---

## 📝 Observações

- O esquema segue boas práticas de normalização.
- Nomes de tabelas e colunas foram padronizados em **letras minúsculas** e com **underline** para maior legibilidade.
- Caracteres especiais (como ç e ã) foram evitados para manter compatibilidade internacional.

---

## 👩‍💻 Desenvolvido por

Projeto desenvolvido por [Karin] como parte do curso **Randstad - Análise de Dados (DIO)**.

---

## 📎 Licença

Este projeto está sob a licença MIT – sinta-se à vontade para usar e adaptar para fins acadêmicos ou profissionais.
