# Sistema de Gestão de Fornecedores e Produtos :package:

Este projeto foi desenvolvido com o propósito de criar um sistema de gerenciamento para fornecedores e produtos, permitindo o cadastro, edição, exclusão e consulta de informações sobre fornecedores e os produtos fornecidos por eles.

### Visão Geral do Projeto

O sistema foi desenvolvido com o objetivo de facilitar a gestão de fornecedores e seus respectivos produtos, proporcionando uma interface simples e eficiente. A estrutura do banco de dados e a aplicação foram projetadas para atender às necessidades básicas de uma empresa que precisa gerenciar seus fornecedores e produtos de forma organizada.

### Tecnologias Utilizadas

- **PHP:** Linguagem de programação principal para a implementação da aplicação.
- **MySQL / MariaDB:** Sistema de gerenciamento de banco de dados utilizado para armazenar as informações de fornecedores e produtos.
- **HTML:** Para estruturação das páginas e apresentação de informações.
- **CSS:** Para estilização da interface do usuário.
  
## Etapas do Desenvolvimento

### 1. Planejamento e Estruturação

No início, discutimos os requisitos do sistema e definimos as principais funcionalidades que o sistema deveria ter. O objetivo foi criar uma aplicação simples, mas eficiente, com as seguintes características:
- **Cadastro de Fornecedores:** Permite o registro de informações sobre os fornecedores, como: nome, e-mail, telefone e imagem.
- **Cadastro de Produtos:** Permite o registro de produtos, incluindo: fornecedor, nome, descrição, preço e imagem.
- **Listagem:** O sistema possibilita a consulta de fornecedores e produtos cadastrados.

### 2. Desenvolvimento do Banco de Dados

Para garantir a eficiência e a integridade dos dados, o banco de dados foi estruturado da seguinte forma:

#### Tabelas

- **fornecedores**: Armazena informações sobre os fornecedores (nome, telefone, e-mail, etc).
- **produtos**: Armazena as informações dos produtos (nome, descrição, preço, fornecedor, e está relacionada ao fornecedor através de uma chave estrangeira).

#### Relacionamento entre Tabelas

Cada **produto** é vinculado a um **fornecedor**, estabelecendo uma relação de um para muitos, ou seja, um fornecedor pode fornecer vários produtos.

### 3. Desenvolvimento do Sistema PHP

A aplicação foi desenvolvida com PHP para permitir a interação entre o usuário e o banco de dados. As principais funcionalidades incluem:

- **Cadastro de Fornecedores e Produtos:** Formulários para adicionar novos fornecedores e produtos.
- **Edição de Fornecedores e Produtos:** Permite a atualização de dados dos fornecedores e produtos já cadastrados.
- **Exclusão de Fornecedores e Produtos:** Funcionalidade para remover registros do banco de dados.
- **Consulta de Fornecedores e Produtos:** Permite visualizar a lista de fornecedores e produtos cadastrados.

### 4. Interface de Usuário

A interface foi desenhada para ser simples e intuitiva. A navegação permite que o usuário acesse rapidamente as principais funcionalidades do sistema, como:
- **Cadastro de Fornecedores**
- **Cadastro de Produtos**
- **Listagem de Fornecedores**
- **Listagem de Produtos**

Cada página foi projetada para ser clara e direta, com foco na usabilidade.

### 5. Implementação de Segurança

Algumas medidas de segurança foram implementadas, como a utilização de **prepared statements** com PDO para evitar SQL Injection e o **validador de dados** nos formulários para garantir a integridade das informações inseridas.
