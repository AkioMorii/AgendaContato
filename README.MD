Projeto desenvolvido em C# MVC exibindo uma pag�na simples de um CRUD de contatos.
O banco de dados usado foi o Postgre e a query �:
	CREATE TABLE CONTATOS (
		Id SERIAL PRIMARY KEY,
		Nome VARCHAR(100) NOT NULL,
		Apelido  VARCHAR(100),
		CPF VARCHAR(11) NOT NULL,
		Telefone VARCHAR(9) NOT NULL,
		Email VARCHAR(250),
		DataCadastro TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
		UltimaAlteracao TIMESTAMP DEFAULT CURRENT_TIMESTAMP
	);

Para utilizar o projeto:
	- Clonar para uma pasta;
	- Intalar depend�ncias (Microsoft.EntityFrameworkCore, Npgsql, Npgsql.EntityFrameworkCore.PostgreSQL);
	- Criar o banco de dados usando a query escrita;
	- Acessar o arquivo appsettings.json e colocar as especifica��es do seu BD em "DefaultConnection";
	- Rodar o projeto.
