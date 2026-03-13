# Biblioteca – Banco de Dados SQL

Este projeto apresenta a criação de um **banco de dados relacional simples para gerenciamento de uma biblioteca**, desenvolvido utilizando **SQL (Oracle)**. O objetivo é praticar conceitos de **modelagem de dados, criação de tabelas e aplicação de constraints** para garantir a integridade das informações.

## Estrutura do Banco

O banco possui **3 tabelas principais**:

### 📚 LIVRO

Armazena informações dos livros da biblioteca.

Campos principais:

* `IDLIVRO` – Identificador do livro (Primary Key)
* `TITULO` – Título do livro
* `AUTOR` – Autor do livro
* `ANO` – Ano de publicação
* `STATUS` – Situação do livro (`D` = Disponível / `E` = Emprestado)

---

### 👤 LEITOR

Armazena os usuários da biblioteca.

Campos principais:

* `IDLEITOR` – Identificador do leitor (Primary Key)
* `NOME` – Nome do leitor
* `TELEFONE` – Telefone de contato
* `EMAIL` – Email do leitor (único)

---

### 📄 EMPRESTIMO

Registra os empréstimos de livros.

Campos principais:

* `IDEMP` – Identificador do empréstimo (Primary Key)
* `DATAEMP` – Data do empréstimo
* `DATADEV` – Data de devolução
* `IDLIVRO` – Livro emprestado (Foreign Key)
* `IDLEITOR` – Leitor responsável (Foreign Key)

---

## Relacionamentos

* Um **livro** pode ter vários empréstimos.
* Um **leitor** pode realizar vários empréstimos.

---

## Tecnologias Utilizadas

* **Oracle Database**
* **SQL (DDL)**

---

## Onde Executar

Este script SQL pode ser executado em ambientes como:

* **Oracle Live SQL**
* **SQL Developer**
* **Oracle Database local**
* Plataformas online de prática SQL compatíveis com Oracle.

Basta copiar o código SQL e executar o script para criar as tabelas no banco de dados.

---

## Autor

Lucas Antunes
Estudante de programação e desenvolvimento de software.
