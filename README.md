<div align="center">
  <img width="200"
    alt="Java Logo"
    src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original.svg"
    />
  <h1>Estudando Banco de Dados com PostgreSQL</h1>
  Repositório de estudos para PostgreSQL.
</div>

## O que é um Banco de Dados?
Resumidamente, um banco de dados é um conjuto de tabelas as quais armazenam as informações. E cada tabela está contida em um banco de dados.

Além disso, pode haver um sistema com vários bancos de dados. Chamado Sistema Gerenciador de Banco de Dados:\
**SGBD**

Pode ser controlado por:
- Programa de Administração (Caso queira administrar);
- Programa Cliente (Caso queira usar);

Conectados por uma conexão via rede.\
Ambos executam tarefas atráves da Linguagem SQL.

```
SELECT * FROM clientes;
```

Existem alguns tipos der bancos de dados, como os bancos de dados relacionais, por exemplo:
- MySQL;
- PostgreSQL;
- SQLite;
- Microsoft SQL Server;
- Oracle;

## Como baixar o postgreSQL?
Pelo windows você pode entrar pelo site.\

Pelo linux(Ubuntu), você pode seguir esse procedimento:
https://youtu.be/cdhpmaa4YJE?si=ZTrlQnpYAwVzd3v-

Caso ocorra algum problema, ao instalar o postgresql, invés de postgresql-15, coloque 16.


## Alguns termos técnicos
- PK AI - Chave primária para cada indivíduo
- NN (Not Null) - Rejeitar um registro sem valor para essa coluna. 
- Self Join - Categorias "recursivas"


## Comandos usando Postgres
Não sei se são comandos gerais ou só pelo ubuntu, mas vou anotar os comandos depois de baixar, etc

psql - ativa os postgres
\password (nome do usuario) - vc muda a senha 

1. sudo -u postgres psql - entrar no postgres (acho que quando ja criado)
2. \l - listar todos os databases
3. CREATE DATABASE (nome do database)- autoexplicativo
4. \c (nome do database) - conectando ao database
5. \dt - exibir as tabelas do database
6. CREATE TABLE funcionários (id SERIAL PRIMARY KEY, name VARCHAR(50), birth DATE) - cria uma tabela com nome **funcionários**, id serial(identificador da tabela), daí em diante são as colunas que eu posso criar
